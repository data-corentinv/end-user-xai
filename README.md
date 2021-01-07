# EUCA: <ins>E</ins>nd-<ins>U</ins>ser-<ins>C</ins>entered Explainable <ins>A</ins>I Framework


The EUCA framework is a **prototyping tool** to design explainable artificial intelligence for non-technical end-users.

<<<<<<< HEAD
It can help you build a low-fidelity explainable AI (XAI) prototypequicklyquickly (without the need to implement), so that you can "trial and error" using the prototype , and implement it as a functional one. 
=======
It can help you build a low-fidelity explainable AI (XAI) prototype, so that you can use it to quickly "trial and error" (without the effort to implement it), and co-design and iterate it together with your end-users.
>>>>>>> fbb0489091b4db167b6bffe77a616600d601b55f

You can use the prototype at the initial phase for user need assessment, and as a start for your explainable AI system iteration.

# Why explainable AI?


![When and why explainable AI for end-users](fig/why_xai.jpg)

As AI is getting pervasive and assists users in making decisions on **critical tasks**, such as autonomous driving vehicles, clinical diagnosis, financial decisions, legal and military judgment, or something crucial that relates to people's life or money, the end-users will be more likely to require AI to justify its prediction.

Making AI explainable to its end-users is challenging, since end-users are **laypersons** or **domain experts**, and they do not have technical knowledge in AI or computer science to understand how AI works.

# Who use EUCA?
EUCA can be used by **anyone who designs or builds** an explainable AI system **for end-users**, such as UI/UX designers, AI developers, AI researchers, and HCI researchers. 

---

# What is the EUCA framework?

![The five main components of EUCA framework](fig/euca_compo.jpg)

The main component of EUCA is the **12 end-user-friendly explanatory forms**, and
- their associated design examples/templates
- corresponding algorithms for implementation, and 
- identified properties (their strength, weakness, UI/UX design implications, and applicable explanation needs) from our user study findings 
See **[explanatory forms page](explanatory_form.md)** for the above details and design examples.

In addition, EUCA also provides a [suggested prototyping method](#prototyping), and end-users' diverse **[explanation need analysis](need.md)** (such as to [calibrate trust](need.md/#trust), [detect bias](need.md/#bias), [resolve disagreement with AI](need.md/#unexpected)).

The 12 explanatory forms in EUCA framework are:
## [Feature-based explanation](explanatory_form.md/#feature)  
1. [Feature Attribute](explanatory_form.md/#fa)  
2. [Feature Shape](explanatory_form.md/#fs)  
3. [Feature Interaction](explanatory_form.md/#fi)  

## [Example-based explanation](explanatory_form.md/#example)  
4. [Similar Example](explanatory_form.md/#se)  
5. [Typical Example](explanatory_form.md/#te)  
6. [Counterfactual Example](explanatory_form.md/#ce)  

## [Rule-based explanation](explanatory_form.md/#rule)  
7. [Rule](explanatory_form.md/#rl)  
8. [Decision Tree](explanatory_form.md/#dt)  

## [Supplementary information](explanatory_form.md/#suppl)  
9. [Input](explanatory_form.md/#input)  
10. [Output](explanatory_form.md/#output)  
11. [Performance](explanatory_form.md/#perf)  
12. [Dataset](explanatory_form.md/#data)  

![end-user-friendly explanatory forms include explaining using feature, example and rule](fig/et.jpg)


---
# <a name="prototyping"></a> How to use EUCA for XAI prototyping?

![The five main components of EUCA framework](fig/euca_workflow.jpg)

## Step 1: Create prototyping cards from explanatory forms
### 1.1 Think about your input and feature data type

The input data and feature format need to be human-understandable, so that end-users can interpret the explanations which are formed by features, examples, or rules.

### 1.2 Get familiar with the [end-user-friendly explanatory forms](explanatory_form.md)  
There are 12 end-user-friendly explanatory types in the EUCA framework. They are grouped into four categories: explaining using features, examples, rules, and supplementary information. The explanatory types are building blocks, and you can combine them to construct your end-user-oriented XAI prototype.

### 1.3 Manually extracting several interpretable features

Given the AI task and input/output data type, the designer starts by manually extracting several interpretable features. 

For example, for tabular data, the features could be the column names that describing the input, such as house size, age, and location. 

For image data, the features could be saliency image part or object for recognition, such as cars, traffic signs, or pathological appearance of a disease on chest X-ray. 

As quick prototyping, the feature content may not necessarily reflect the true content generated by XAI algorithms. They served as content placeholders for the prototyping card design template.

### 1.4 Fill in the prototyping card template with the extracted features

You can use the **[prototyping card design templates](#template)**, and fill in the template with the above extracted features. In this way, you created the prototyping card for each explanatory form. You can regard them as individual components of your future explainable AI prototype. 

In the design template and example, we provide the basic visualization of the explanatory forms used in the user study. You can also create their own template from scratch by referring to the possible **Visual Representation** part for each [explanatory form](explanatory_form.md). 

### 1.5 (optional) Prepare multiple cards varying UI/UX

For a particular explanatory form, you may prepare multiple versions varying the visual representations (e.g.: graphics or text) and UI layout, alternating contents from brief to details, and providing different options, such as whether to use pre-defined or user-defined contrastive outcome on counterfactual example, whether to give users the option to set a threshold level for feature attribute.

You may get more inspirations from the **Design Implication** part in the [end-user-friendly explanatory forms](explanatory_form.md). 

Each explanatory form and its variations are presented on individual prototyping cards.

### 1.6 (optional) Consider applying the general human-AI interaction guidelines in your design

While designing UI/UX variations for the prototyping cards, designers may also consider and apply the general [human-AI interaction guidelines](https://www.microsoft.com/en-us/research/uploads/prod/2019/01/Guidelines-for-Human-AI-Interaction-camera-ready.pdf), such as the following selected design guidelines that are more relevant to XAI system: 
- remember recent interactions
- support efficient invocation, dismissal and correction
- remember recent interactions
- learn from user behavior
- encourage granular feedback

## Step 2:  Co-design and iterate low-fidelity prototype with end-users
The EUCA framework aim to facilitate your participatory design process, i.e., to involve end-users or other stakeholders in the software development lifecycle. 

### 2.1 Understanding end-users' needs for explainability
You can use the prepared explanatory form prototyping cards to discuss with your users about their needs for explainability in detail. Sometimes the motivation or trigger point to check explanations vary from calibrating trust with the AI system, to verifying the decisions from AI, to improving the predicted outcomes. And the demands for explainability may be distinct for different explanatory purposes. And users need may vary in different scenarios. Before your talk with the stakeholders, you may skim through the **[explanation need analysis](need.md)** to have a general idea.

### 2.2 Talk with end-users

In the meeting with end-users, to quickly create a low-fidelity paper prototype from the prototyping cards, your end-users can select, rank, combine, modify the prototyping cards, and even sketch new ones. In this process, you may ask users why they selected or did not select a card, and their rationals for making such a card combination, whether the combination will fulfill their requirements, and what is lacking in the current prototype. 

Your users can easily manipulating the card positions to try out different layouts to examine different UI design possibilities (for example, on brewers, tablet or mobile phone).

Users can also comment on and revise each variation of the same explanatory form. With the tangible prototyping card examples, designers can know in-details about users specific requirements on the UI/UX design.

The prototyping cards may facilitate the discussion of UX design, for examples, users may choose to hide some cards and only show them on-demand, or to present different explanatory information in different contexts. 

After the initial communication with users, you need to synthesize users comments and decide one or several prototype designs (such as using majority voting). Then based on the prototyping card ranking and combination, you can create low-fidelity prototypes, and continue to seek user and/or other stakeholders' feedback and iterate the prototype. 

During the above process, you may refer to the user study findings to be informed about the properties of the explanation forms (pros, cons, applicable explanation needs, and design implications in [explanatory forms](explanatory_form.md)).

## Step 3:  Implement a functional prototype
We list the corresponding algorithms after each explanatory form, so that you or the technical partner can implement them or use the existing [open-sourced implementation](explanatory_form.md/#os) to deploy your XAI prototype. You may continue to iterate your XAI system based on the implemented working prototype. 

---

# <a name="template"></a> Prototyping materials for download
We provide the following prototyping materials:
1. Templates: Blank cards card grids with their explanatory type name
2. Examples: We demonstrate creating prototype for tabular or sequential input, and for image input respectively. 
* **House**: House price prediction. Tabular input data
* **Health** : Diabetes risk prediction. Sequential or tabular input
* **Car**: Self-driving car. Image or video input
* **Bird**: Bird species recognition. Image input

We have the following versions:
- [Sketch file](https://github.com/weinajin/end-user-xai/blob/master/prototyping/EndUserXAI_template.sketch)
- PDF print version: [template](https://github.com/weinajin/end-user-xai/blob/master/prototyping/EndUserXAI_Template.pdf),   [blank card](https://github.com/weinajin/end-user-xai/blob/master/prototyping/EndUserXAI_BlankTemplate.pdf),   [all templates with individual card examples](https://github.com/weinajin/end-user-xai/blob/master/prototyping/EndUserXAI_Template_all.pdf)    
- [PowerPoint (Coming soon)]() 
- [Google slides (Coming soon)]()

You can create your own or even draw your explanatory cards on paper.  We provide some examples on tabular and image input data for your reference.

---

# <a name="cite"></a> How to cite the EUCA framework?
[Research paper]()

---

# <a name="share"></a> I used EUCA and I want to share my XAI design

You can inspire other designers by sharing your sketches, designs and prototypes using EUCA. We will post your design on the EUCA page.

To share your design, please feel free to contact weinaj at sfu dot ca, or open a pull request on the [EUCA project repo](https://github.com/weinajin/end-user-xai).


