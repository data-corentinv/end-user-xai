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


### Pros

Users can **intuitively understood** feature attribute, and would likely accept it as an explanation.

>*" It uses a simple way to highlight the most important parts, and you can see very clearly at your first sight how this can be recognized."* 
> *"It's easy to read. ...And you have a bar (chart) here it's really clear information that people understand instantly."*

By showing *"finer details"* (P10) and *"breakdown and weights of features"_(P23) *"that AI took into account"_ (P31), participants perceived \[feature attribute\]{style="color: orange"} **can answer *"how"* and *"why"* questions**.

*"tells me why"_(P20), *"gives me the behind the scenes"_ (P24), *"tells me how AI read things and how it makes decisions"* (P03), *"have an understanding of how much weight AI is giving to each of the factors"* (P22), and *"identify key aspect, ...support its reasoning"* (P18).

### **Applicable Explanation Needs**

By checking feature importance ranking, participants would instantly *"compare with my own judgment, to see if that aligns with my feature attribute"* (P01, Car, \[Safety\]{style="color: blue"}), especially when participants need to **verify AI's decision**.

### **Cons**

Although a causal relationship may not be confirmed, some participants tended to **assume \[feature attribute\]{style="color: orange"} is causal**, or simplify the relationship among features by assuming they are **independent from each other**. This was usually occurred when they were seeking explanation to \[improve the predicted outcome\]{style="color: blue"}. And participants were likely to be informed by the feature importance score to prioritize the most important features to take actions upon.

*"Seeing that body weight is more important than exercise, I think I will focus on changing what I ate, instead of like responding by going to the gym everyday."* (P16, Health, \[Improvement\]{style="color: blue"}) -- Relies on \[feature attribute\]{style="color: orange"} to improve the outcome.

*"It (\[feature attribute\]{style="color: orange"}) shows what are the most important factors that AI has taken into account, so you could target the biggest factors."* (P31, Health, \[Improvement\]{style="color: blue"}) -- Assumes a causal relationship and prioritizes the action.

*"If my blood sugar puts me at a super high risk here, but my caloric intake doesn't actually put me at that higher risk, it's like a lower risk, then I would rather just focus on blood sugar. "* (P22, Health task) -- Ignores the complex interaction between blood sugar and caloric intake.

### **Design Implications**

To avoid the above causal illusion, UI/UX design may need to **alarm users** either implicitly or explicitly that changing the important features may not necessarily lead to the outcome change in the real world, due to correlation does not necessarily imply causality.

For designing UI/UX of its prototyping card, designers may consider **varying different representations** of the feature importance, such as showing the feature ranking only and allowing users to check the detailed attribute scores on demand, or allowing users to set a threshold on the attribute score and only showing features above the cut-off value, as suggested by a few participants.

*"If the percentage (of the feature) is below the cutoff value, the users does not need to see (the feature), reduce the cognitive load."* (P04, Bird, \[Learning\]{style="color: blue"})

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

