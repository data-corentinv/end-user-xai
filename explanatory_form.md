# End-User-Friendly Explanatory Forms

We identify end-user-friendly explanatory forms from technical literature. By end-user-friendly we mean the users are not required to have technical knowledge to understand the explanation.

**Index**

* [Feature-based explanation](#feature)  
1. [Feature Attribute](#fa)  
2. [Feature Shape](#fs)  
3. [Feature Interaction](#fi)  

 * [Example-based explanation](#example)  
4. [Similar Example](#se)  
5. [Typical Example](#te)  
6. [Counterfactual Example](#ce)  

* [Rule-based explanation](#rule)  
7. [Rule](#rl)  
8. [Decision Tree](#dt)  

* [Supplementary information](#suppl)  
9. [Input](#input)  
10. [Output](#output)  
11. [Performance](#perf)  
12. [Dataset](#data)  

—

# <a name="feature"></a>1. Feature-based explanation

Feature-based explanations are the most common form of explanation information. 

We refer _feature_ to a piece of information that is carried out by the input data. For example, a real estate agent can describe a house by its size, location, and age, three descriptive features; The feature of an image can be the individual pixels, a car object highlighted, or an explicit concept of "car". 

To use features for explanations, the feature representation must be human-interpretable. 

The feature-based explanations consist of three explanatory forms:

## <a name="fa"></a> 1.1 Feature Attribute


It indicates which features are important for the decision, and what are their attributions to the prediction. For example, it can be a list of key features and their importance scores to the house price prediction, or a color map overlaid on input image indicating the important parts/objects for the recognition. It assumes the prediction is explainable by linearly addable important features.

### Visual representation

![Feature_attribute](prototyping/Feature_attribute.png)

Its visual representation largely depend on the data type of the features. For image and text data, overlaying a **saliency map** or color map on the input is the common visualization. It uses sequential colors to code the fine-grained feature importance score for individual feature (could be pixels for an image input, words for text data). For image/video input data, other popular visualizations include using _masks_, _segmentation maps_ or _bounding boxes_ on the saliency objects.

To visualize multiple feature attributes for tabular or text data, a **bar chart** is typical choice. The variations of bar plot include waterfall plot, treemap, wrapped bars, packed bars, piled bars, Zvinca plots, and tornado plot. _Box plot_ can be used to visualize the distribution of the feature importance score. Its variations include violin plot and beeswarm plot that show more detailed data distribution and skewness.

## <a name="fs"></a> 1.2 Feature Shape


It shows the relationship between one particular feature and the outcome, such as the house size to the predicted house price. Usually, it is presented as a line plot (for continuous feature) or a bar plot (for categorical feature), depicting whether the relationship between the outcome and a feature is monotonic, linear, or more complex.

### Visual representation

![Feature_shape](prototyping/Feature_shape.png)

**Line plot** and _scatter plot_ are common visualizations to show the effect of an individual feature to the predicted outcome.

## <a name="fi"></a>1.3 Feature Interaction



When features interact with each other, their total effect on the outcome may not be a linear sum of each individual effect. \[Fi\]{style="color: orange"} considers such interaction and shows the total effect of two or three features to the outcome. It can be regarded as an extension of \[fs\]{style="color: orange"} by taking two or more features into account.

### Visual representation

![Feature_interaction](prototyping/Feature_interaction.png)

**2D or 3D heatmap** is used to visualize the effect of feature interactions on the predictions. Limited by the visualization, the heatmap can only show interaction for at most three features (using 3D heatmap). More complicated multiple paired feature-feature interactions can be visualized using matrix heatmap, node-link network, or contingency wheel.

—

# <a name="example"></a>2. Example-based explanation

Human uses examples to learn and explain. Examples carry contextual information and are intuitive for end-users to interpret. Three different types of examples are included:

## <a name="se"></a>2.1 Similar example

Similar examples are instances that are similar to the input data regarding their features in the feature space.
![Similar_example](prototyping/Similar_example.png)


## <a name="te"></a> 2.2 Typical example

A typical or prototypical example is a representative instance for a certain prediction. For example, a typical example of the diabetes prediction could be a patient who exhibits the typical features (abnormal hemoglobin A1C level) used by clinicians to diagnose diabetes.

### Visual representation 

![Typical_example](prototyping/Typical_example.png)

For similar and typical examples, it is straightforward to show several the examples with their corresponding predictions.

## <a name="ce"></a>2.3 Counterfactual example

Its features are similar to the input, but has minimal feature changes so that its prediction is distinct from the input. 

For example, an instance C that is predicted as healthy is a counterfactual example for the input I that is predicted to have diabetes, if C has all the same features as I, except its blood sugar level is lower than I. 

### Visual representation 

![Counterfactual_example](prototyping/Counterfactual_example.png)

Counterfactual examples can be shown as two instances with their **counterfactual/contrastive features highlighted**, or a **transition** from one instance to the other by gradually changing the counterfactual features.

—

# <a name="rule"></a> 3. Rule-based explanation
Rule-based explanations are explanations where decisions of the model, in whole or in part, can be described succinctly by a set of logical if/else statements, mimicking human reasoning and decision making. It also implies the decision boundary thus may be convenient for counterfactual reasoning. The rule-based explanation is a global explanation of the model's overall behavior. It includes the following explanatory forms. We note rule and decision tree actually carry out similar explanation information. But since they are usually generated by different XAI algorithms, and their representation format (text vs. diagram) are distinct to the end-users, we separate the two explanatory forms.


## <a name="rl"></a>3.1 Rule text

The decision rules or decision sets are simple IF-THEN statement with condition and prediction. For example: IF blood sugar is high, AND body weight is over-weighted, THEN the estimated diabetes risk is over 80%.

### Visual representation

![Decision_rule](prototyping/Rule.png)


Rules are usually represented using **text**. Other representing formats include table \[@Castro2019\] or matrix \[@Ming2019\] to easily align and compare rule clauses.

## <a name="dt"></a> 3.2 Decision tree

Rule is represented graphically as a tree structure, with the branch representing the decision pathway, and the leaf is the outcome.

### Visual representation

![Decision_tree](prototyping/Decision_tree.png)


The most common representation is to use a node-link **tree diagram**. other visual representations to show the hierarchical structure include treemap, cladogram, hyperbolic tree, dendrogram, and flow chart.

—

# <a name="suppl"></a> 4. Supplementary information

In addition to the above explanatory forms generated by XAI algorithms, an XAI system needs to present some necessary supplementary information to the end-users, such as input, output, decision confidence/certainty, model performance metrics, training dataset information such as data distribution, etc. We included the following essential and common ones in our framework, and indicates whether they are global (explaining the model's overall behavior) or local explanation (explaining the decision to the individual instance):

## <a name="input"></a> 4.1 Input

Input is end-users' input data. Input is local explanation.

![Input](prototyping/Input.png)


## <a name="output"></a> 4.2 Output

![Input](prototyping/Input.png)


Output is AI's prediction on the input. It is local explanation.

Sometimes the output prediction is accompanied by **decision certainty** level. Since the prediction from AI models is usually probabilistic, the certainty score shows the case-specific certainty level about how confident model is in making this particular decision. The certainty is local information on the particular prediction.

## <a name="perf"></a> 4.3 Performance

![Performance](prototyping/Performance.png)


Performance metrics (such as accuracy, confusion matrix, ROC curve, mean squared error) help end-users to judge the overall decision quality of the model, and to set a proper expectation on the model's capability. It is global information about the overall performance of the model. 


## <a name="data"></a> 4.4 Dataset

![Dataset](prototyping/Dataset.png)

Dataset information includes the metadata on the dataset where the model is trained on, such as data distribution, may help end-users to understand the model and identify potential flaws in the data.

# Open-sourced XAI software packages
[Alibi](https://docs.seldon.io/projects/alibi/en/v0.2.0/overview/getting_started.html)

[Software list1](https://github.com/lopusz/awesome-interpretable-machine-learning#software)

[Softwareblist 2](https://github.com/jphall663/awesome-machine-learning-interpretability#explainability--or-fairness-enhancing-software-packages)

[Captum, a pytorch XAI library](https://captum.ai/) 

