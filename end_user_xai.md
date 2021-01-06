# EUCA: The End-User-Centered Explainable AI Framework


The EUCA framework is a prototyping tool to design explainable AI for non-technical end-users.
It can help you quickly build a low-fidelity XAI prototype. You can use the prototype at the initial phase for user need assessment, and as a start for your XAI system iteration.

## Target audience
Anyone who designs or builds an explainable AI system, such as UX designer, AI developer, and AI researcher. The framework is especially useful if your XAI system is for users who have no technical knowledge of AI, machine learning, data science, or programming.

## What is EUCA framework?
The EUCA framework contains 12 types of explanations that are end-user-friendly, meaning users are not required to have the technical knowledge to understand these explanations. This is suitable if your XAI system is designed for non-technical end-users.

The 12 explanation types in EUCE framework are:
### Feature-based explanation
1. [Feature attribute](#fa)
2. Feature shape
3. Feature interaction
### Example-based explanation
4. Similar example
5. Typical example
6. Counterfactual example
### Rule-based explanation
7. Rule text
8. Decision tree
### Supplementary information
9. Input
10. Output
11. Performance
12. Dataset

See [below](#euce) for their details and examples.


## How to use the EUCA framework for XAI prototyping?
### Step 1: Think about your input and feature data type
The input data and feature format need to be human-understandable, so that end-users can interpret the explanations which are formed by features, examples, or rules.

### Step 2:  Get familiar with the end-user-friendly explanatory components 
There are 12 end-user-friendly explanatory types in the EUCA framework. They are grouped into four categories: explaining using features, examples, rules, and supplementary information. The explanatory types are building blocks, and you can combine them to construct your end-user-oriented XAI prototype.
The components in the EUCA framework are introduced [here](#framework).


### Step 3:  Create your explanatory component cards

Our [design templates](#template) contain the 12 explanatory components, each one is presented on a card. You can adopt the explanatory components to your task, and regarded them as individual components of your explainable AI prototype. 

For one explanatory component, you may prepare multiple versions varying its visual design, layout, the degree of details, etc. You may get more inspirations from the **design implication** part of each explanatory component. 


### Step 4: Talk to your end-users or other stakeholders, select and combine the explanatory components to construct your prototype
The EUCA framework can facilitate your participatory design process, i.e., to involve end-users or other stakeholders in the software development lifecycle. You can use the prepared explanatory component cards to discuss with your users about their needs for explainability. Sometimes the purposes to check explanations vary from calibrating trust with the AI system, to verifying the decisions from AI, to improving the predicted outcomes. And the demands for explainability may be distinct for different explanatory purposes. In your discussion, your users can select, combine, and arrange the explanatory cards to form a paper-based prototype that fulfills their needs under different purposes of checking explanations. 


### Step 5: Deploy and iterate the prototype
We list the corresponding algorithms after each explanatory component, so that you can implement them or use the existing open-sourced implementation to deploy your XAI prototype. You can iterate your XAI system based on the implemented working prototype. 




## Prototyping materials for download
We provide the following prototyping materials:
1. Templates: Blank cards card grids with their explanatory type name
2. Examples: We demonstrate creating prototype for tabular or sequential input, and for image input respectively. 
* **House**: House price prediction. Tabular
* **Health** : Diabetes risk prediction. Sequential or tabular input
* **Car**: Self-driving car. Image or video input
* **Bird**: Bird species recognition. Image input

We have the following versions:
- [Sketch file]()
- [PDF print version]()      
- [PowerPoint]() 
- [Google slides]()

You can create your own or even draw your explanatory cards on paper.  We provide some examples on tabular and image input data for your reference.


## How to cite the EUCE framework?
[Research paper]()


## Why explanations?

![When and why explainable AI for end-users](fig/why_xai.jpg)

The explanation is a necessary component of an AI system, if users use the AI to perform critical tasks that may have serious impacts on people's life, money, career, etc.





## EUCE: End-User-Centered Explainable AI Framework

### Feature-based explanation
1. {#fa} Feature attribute
2. Feature shape
3. Feature interaction
### Example-based explanation
4. Similar example
5. Typical example
6. Counterfactual example
### Rule-based explanation
7. Rule text
8. Decision tree
### Supplementary information
9. Input
10. Output
11. Performance
12. Dataset



## Open-sourced XAI software packages
[Alibi](https://docs.seldon.io/projects/alibi/en/v0.2.0/overview/getting_started.html)
[Software list1](https://github.com/lopusz/awesome-interpretable-machine-learning#software)
[Softwareblist 2](https://github.com/jphall663/awesome-machine-learning-interpretability#explainability--or-fairness-enhancing-software-packages)
[Captum, a pytorch XAI library](https://captum.ai/) 

