# RQ2: End-Users' General Requirements under Various Explanation Needs {#rq12}

Although participants may have various motivations to check
explanations, two main themes of explanation needs emerged in the
interview. Quantitative clustering analysis confirmed similar trends as
visualized in
Fig. [\[fig:purpose\_cluster\]](#fig:purpose_cluster){reference-type="ref"
reference="fig:purpose_cluster"}.

The first and fundamental driving force of checking explanations is to
**verify AI's prediction**, and to gain trust and understanding.

*"Like boyfriend and girlfriend, I want to know what my boyfriend is
thinking. Similarly, I want to know what the car's thinking before I'm
with the car."* (P32, Car task, [Safety]{style="color: blue"}) -- To
gain understanding on AI

*"I will also want to know how the software can predict the 80% chance
that I'm going to have diabetes. And also, how did they come up with
that numbers? Just giving me a number without justification or some
verifiable reasons, it's just unlikely I would accept it because it may
not be true."* (P25, Health task, [Trust]{style="color: blue"})

The following purposes are more related to this motivation: calibrating
[trust]{style="color: blue"} (Section [2.1](#trust){reference-type="ref"
reference="trust"}), ensuring [safety]{style="color: blue"}
([2.2](#safety){reference-type="ref" reference="safety"}), detecting
[bias]{style="color: blue"} ([2.3](#bias){reference-type="ref"
reference="bias"}), and resolving [disagreement]{style="color: blue"}
([\[unexpected\]](#unexpected){reference-type="ref"
reference="unexpected"}).

The second motivation to check explanations is for **personal
improvement**, i.e.: to improve users' own welfare, such as to enhance
personal problem solving skills and learning, or to improve the
predicted outcome. This is built upon the trust and verification from
previous experience, as one participant stated:

*"(When trust has been established,) what has to be done in the next
phase of the (AI) software, is how the software is being helpful to me.
\...If I know the result, I don't think I would want to dig in to see
why it is, but I would want to see how I can reduce the chances of
diabetes."* (P23, Health)

The following purposes are more related to this motivation: to seek
suggestions to [improve the
outcome]{style="color: blue"}([2.8](#control){reference-type="ref"
reference="control"}), to [learn]{style="color: blue"} and discover new
knowledge ([2.7](#learn){reference-type="ref" reference="learn"}), to
[differentiate]{style="color: blue"} similar instances
([2.6](#differentiate){reference-type="ref" reference="differentiate"}),
to facilitate verbal ([Communication]{style="color: blue"},
[2.9](#communicate){reference-type="ref" reference="communicate"}) and
written communication ([Report]{style="color: blue"},
[2.10](#report){reference-type="ref" reference="report"}), and to
balance among [multiple objectives]{style="color: blue"}
([2.11](#multi){reference-type="ref" reference="multi"}):

[**Calibrate trust**]{style="color: blue"} {#trust}
------------------------------------------

The process of calibrating trust involves multiple factors and their
complicated interactions. We summarize the following key emerged themes
participants requested to calibrate their trust toward AI.

1.  **Performance** Trust towards AI is fundamental to incorporate AI's
    opinion into the critical decision-making process [@Yu2019], and
    many explanation needs below are built on trust.

    Since end-users usually do not have complete computational and
    domain knowledge to judge AI's decision process, model performance
    becomes an important surrogate to establish trust.

    *"Even if AI tells me how it reaches its decision, I cannot judge
    whether it's correct since it is a medical analysis and requires
    professional medical knowledge. I just know the accuracy and that'll
    be fine."* (P01, Health)

    Prior work identified two types of performance: stated and observed
    performance [@Yin2019], and they were both mentioned in the
    interview. *Stated performance* or accuracy is performance metrics
    tested on previous hold-out test data, and it was mentioned by most
    participants as a requirement to build model trust.

    *"I understand maybe AI is learning from past examples, and it may
    be finding patterns in the data that might not be easy to explain.
    So I'm less concerned about how it's getting there. I think I do
    have a trust that is doing it right, as long as there's something
    you can test after how accurate it's been. "* (P16, Health)

    Compared to assessing the performance metrics, some participants
    tended to test AI by themselves and get hands-on *observed
    performance* to be convinced. This requires users to have a referred
    ground truth from their own judgment or reliable external sources.

    *"(My own test driving experience) is way more useful than watching
    a (test driving) video, because you shouldn't trust everything. The
    video might be just made to wait for you to buy the car. So talking
    from a customer perspective, I would like to try it myself, because
    I also sell things. So I would always like to try it myself instead
    of watching a video."* (P21, Car)

2.  **Feature** The important features that AI was based on are the next
    frequently mentioned information.

    *"I would like to know the list of criteria that the AI chose the
    price based on, and which one weighs more."* (P30, House)

3.  **The ability to discriminate similar instances** This information
    was requested by several participants to demonstrate AI's
    capability.

    *"([Decision tree]{style="color: orange"}) It's showing me that it's
    picking from a few similar ones, not just like a random ray of blue,
    purple, green birds. It's not random, it's a calculated response.
    More of that would help me trust AI."* (P06, Bird)

    *"[Typical example]{style="color: orange"} seems to be pretty good
    at picking up on differences. [Similar
    example]{style="color: orange"} I can see that it's got a good
    variety of similar birds. So I found these ones make me trust it
    more.* (P16, Bird)

4.  **Dataset** The dataset size that AI was trained on is another
    surrogate mentioned by some participants to enhance trust.

    *"To me what artificial intelligence does is just collecting a lot
    of data, and tries to make sense for behavioral patterns. So I would
    actually trust it, because I think it's just based on data, it is a
    more accurate measurement of what market rate is for house prices."*
    (P03, House)

    *"If I know that the AI comes from a large database, it seems like
    the database is actually the experience that AI has. So the larger
    it (dataset) gets, the more experienced AI would be, so I can trust
    it more."* (P30, House)

5.  **External information** This is another surrogate mentioned by
    participants to judge if AI is trustworthy. The external information
    could include:

    1.  Peer reviews, endorsement, and company credit.

        *"Since I'm not really a tech person, so I'm not sure how I look
        at it in a technical way. So that's why I just really depend on
        the company's reputation, and also how people feel about the
        website."* (P28, House)

    2.  Authority approval and liability.

        *"I trust more if the government themselves kind of stands
        behind it, getting some sort of government approval helps it a
        little bit more. So if there's some health authority like Health
        Canada or FDA support gives it more legitimacy."*(P24, Health)

        *"For me personally, I would prefer if an actual person is there
        in the end, at least in the beginning stage. So if somebody is
        there to just say, 'hi, I'm so and so', and then AI takes
        control. Then we still know that there is somebody who's liable
        in the end for whatever happens.''* (P23, Health)

### Preferred explanatory forms {#preferred-explanatory-forms .unnumbered .unnumbered}

The top three most selected forms for the need to [calibrate
trust]{style="color: blue"} were [performance]{style="color: orange"}
(20/40), [output]{style="color: orange"} (20/40), and [feature
attribute]{style="color: orange"} (17/40). This quantitative results
corresponds to the above qualitative themes (Figure.
 [\[fig:mtx\]](#fig:mtx){reference-type="ref" reference="fig:mtx"}).

\centering
![ **Explanatory type---purpose heatmap**. The darkness level and number
in the grid is the percentage of a explanatory type selected for that
purpose []{label="fig:mtx"}](figures/purpose_card.pdf){#fig:mtx
width="80%"}

[**Ensure safety**]{style="color: blue"} {#safety}
----------------------------------------

To ensure safety and reliability of the AI system in critical tasks (the
autonomous driving vehicle task in our study), participants frequently
mentioned **checking AI's performances in test cases**, expecting the
testing to **cover a variety of scenarios** to show the robustness of
safety. Although it is impossible to enumerate a complete list of
potential failure cases in testing, extreme cases or potential accidents
were the main concerns and focuses of end-users.

*"Potential crashes or just like someone speeding or a pedestrian
jumping out of nowhere."* (P19)

*"There is likely to be someone running around, so it needs to show me
the extreme cases. \...I need to see something like FMEA, failure modes
and effects analysis, just to be like, 'okay this is how it works.'
because I know nothing is foolproof. There are always to be something,
but to what extent."* (P03)

Similar to the need to [calibrate trust]{style="color: blue"}, alongside
the above *stated performance*, a few participants required *observed
performance* to emotionally accept AI as an emerging technology.

*"definitely I would want to be in one car. I think information is not
helpful, it's not an intellectual factual thing, it's emotionally not
acceptable. It (AI) is new and I have to learn to trust it"* (P17).

### Preferred explanatory forms {#preferred-explanatory-forms-1 .unnumbered .unnumbered}

Regarding the specified information to present in the performance
testing, participants would like to check the objects detected by AI
([feature attribute]{style="color: orange"}, 9/13):

*"It shows how it detects the important objects and how it makes
decision"* (P03, P05, P27)

*"See if (the [feature attributes]{style="color: orange"}) align with my
own judgment of feature importance."* (P01)

[Performance]{style="color: orange"} (6/13) were also favourable to
check the metrics summary of performance. A specified
[performance]{style="color: orange"} analysis in different test
scenarios may also help as a safety alert by revealing the weakness of
the system.

*"Let's say I'm driving on a rainy day, then I know that I should be a
lot more careful than when I'm with the car in a normal condition."*
(P27)

[Similar example]{style="color: orange"} (7/13) were preferred since it
showed *"what's the condition or what kind of decision the car gonna
make"* (P32), although participants did not focus on its similarity
nature, but rather assumed it can showcase a variety of cases including
the extreme cases. Several participants chose [decision
tree]{style="color: orange"} (6/13) because it *"gave me an overview of
how the car makes decision"* (P27).

[**Detect bias**]{style="color: blue"} {#bias}
--------------------------------------

Participants were concerned about population bias [@Mehrabi2019], or
distribution shift where AI models are applied to a different population
other than the training dataset. Such concern is more prominent when a
prediction is based on users' own personal data, and when users are in
minority subgroups. Participants wanted to compare and see **if their
own subgroup is included in the training data**.

*"I know I'm in a class, they talked about how a lot of studies haven't
been done specifically on women, even though they (diabetes) affect men
and women differently. That is probably something I would want to know
about, like if it gave me this result and then it had a little note that
explained the research was done more on that demographic, so it may be
more true for that demographic, but they're just trying to, what's the
word, extrapolate to this group where I sit."* (P22, female, Health)

Unlike the common bias and fairness problem in AI where the protected
features should not affect the prediction, in our Health task on
diabetes prediction, the protected features (age, gender, ethnicity) do
lead to a difference in diabetes outcome (referred as explainable
discrimination in [@Mehrabi2019]). Participants who were aware of this
point **required AI to account for such differences among subgroups**.

*"I know some ethnic groups just by genetic makeup could be more
predisposed to diabetes. In order for it (AI) to arrive at this
decision, I would think that it has maybe like a sample size of
different people with different ethnicities to try to figure out. I
would think there'll be years and years of research has already been
done of the different groups, different ages that would then be factored
in by AI. If I can see it (AI) is using that information, I'll be a lot
more comfortable to actually using the AI's recommendation."* (P17,
Health)

In cases where the AI task is not related to personal information (in
our study the self-driving car task), participants required AI to be
able to detect objects and perform equally in all potential biased
conditions.

*"Now we are operating in night time, or different weather, but they
(the self-driving cars) still have to be able to see the signs and
identify the objects."* (P13, Car)

### Preferred explanatory forms {#preferred-explanatory-forms-2 .unnumbered .unnumbered}

A fine-grained [performance]{style="color: orange"} (12/24) analysis
based on protected-feature-defined subgroups [@Mehrabi2019] can help
users to identify potential biases.

*"I would want to see the certainty and what the prediction error can
potentially be for my demographic versus other groups. If it (the
prediction error) is quite low, then I would probably worry less about
that"* (P22, Health).

Participants chose [similar]{style="color: orange"} + [typical
example]{style="color: orange"} (12/24, means out of the 24
card-selection responses on [Bias]{style="color: blue"}, 12 selected
either [similar]{style="color: orange"} or [typical
example]{style="color: orange"}) to help inspect the data and model, and
to compare with other similar instances to confirm their subgroup is
included in the model.

*"You would want to know what the data that it's being drawn from, is it
similar to you?"* (P16)

[Feature attribute]{style="color: orange"} (12/24) was also chosen since
participants wanted to check if AI could still detection important
features in minority conditions.

*"I want to see how well AI is performing at night to see what it
detected."* (P05, Car).

[**Unexpected** ]{style="color: blue"}: When Users Disagree with AI
-------------------------------------------------------------------

 [\[unexpected\]]{#unexpected label="unexpected"} When AI's predictions
did not align with participants' own expectations, most participants
would *"question AI"* (P16, P20) and *"the contradiction may let me
confuse"* (P02). Some may lose trust with AI thus would not go further
to check its explanations, if they were confident about their own
judgment. Some would check *"a trusted second opinion"* (P06, P10), or
refer to human experts (P12).

But for the majority of participants, **explanations were needed *"to
know why"*** (P01) and to resolve conflicts.

*"I'm feeling conflicted because it's giving me two different
information, my own personal belief and AI. So in order to convince me
that AI does know what it's talking about, you need to go through the
mental validation step \[pointing to the ranked explanatory cards\]. So
by the time I go through this (explanatory cards) and I come out of it,
I am extremely convinced."* (P24, Health)

Explanations help to identify AI's flaws and reject AI, or to check the
detailed differences and to be convinced and correct user's own
judgment, although *"it might be harder to persuade me"* (P31).
Specifically, participants *"try to understand what makes a difference
(between AI and my prediction)"* (P03), which is similar to the need to
[differentiate]{style="color: blue"}
(Section [2.6](#differentiate){reference-type="ref"
reference="differentiate"}). To show why the predictions are different,
many participants **required a list of key features**.

*"Because AI cannot think like a human, so the reason that I ask for the
criteria list is trying to think how similar to me is AI's thinking. So
maybe AI is thinking better, or is seeing a wider range, so it's
checking things that I've never thought about."* (P03, House)

In case AI made errors, seeing what AI is based on can facilitate user's
"debugging'' process. Although end-users cannot debug the algorithmic
part, they may be able to debug the input to see if AI *"have the
complete information"* (P03) as users have. Furthermore, if some key
input information is lacking in AI's decision, the system needs to allow
users to provide feedback by inputting more information (P03, P24), or
*"correct the error"* (P16) for AI.

### Preferred explanatory forms {#preferred-explanatory-forms-3 .unnumbered .unnumbered}

[Feature attribute]{style="color: orange"}: 28/61, [similar
example]{style="color: orange"}: 25/61, [decision
tree]{style="color: orange"}: 23/61,
[performance]{style="color: orange"}: 20/61.

[Expected]{style="color: blue"}: When Users Agree with AI
---------------------------------------------------------

In contrast, when the prediction matched participants' expectations,
participants *"will trust the AI more"* (P10), and the motivation to
check explanations was *"not as strong as the previous one
([unexpected]{style="color: blue"} purpose)"* (P02). Some participants
stopped at the prediction, willing to accept the "black-box'' AI and may
*"not even waste my time (checking explanations)"* (P20).

A few participants still wanted to check further explanations for the
following motivations:

1.  To **boost user's confident**.

    *"Even in this (expected) scenario, it would be nice to have some
    bullet points, like the reasons behind it the estimation being
    accurate, because if someone says that you're charging me way too
    much, I can have point by point reasons explaining to you why this
    house worth this price, it actually kind of as a confidence boost to
    think you are not overcharging or undercharging."* (P03, House)

2.  To [**improve the outcome**]{style="color: blue"} (see improvement
    Section [2.8](#control){reference-type="ref" reference="control"}
    for more findings).

    *"If diabetes already runs in my family, (and AI predicts my risk of
    diabetes is 80%), it would probably make me more confident about the
    software. So I might want to ask for more information about which
    aspects of my health records were the most important for making this
    decision? Coz then maybe that can help me with my future activities
    and changing things in the future."* (P31, Health)

### Preferred explanatory forms {#preferred-explanatory-forms-4 .unnumbered .unnumbered}

[Feature attribute]{style="color: orange"}: 13/34, [similar
example]{style="color: orange"}: 12/34, [typical
example]{style="color: orange"}: 10/34.

[**Differentiate similar instances**]{style="color: blue"} {#differentiate}
----------------------------------------------------------

To facilitate end-users' need to differentiate similar instances, AI is
required to first have the ability to discern similar instances.

*"Depends on how good it is\...So I think you would have to improve how
AI picks up the birds, like maybe these are the same color birds, but
maybe they have slightly different characteristics. So if AI can pick
that up, then I think it would be better."* (P10)

In case of doubtful prediction, participants expected AI to indicate how
certain it is to the prediction.

*"I would expect AI if it doesn't know, it would give choices. So it
would say 100% or 99% that's an indigo bunting, and 89% it thinks it's a
finch."* (P05)

Based on that, AI needs to be able to *"**pinpoint unique features**
that made them really different from each other"* (P06). In addition,
the interface may also need to support users' own comparison.

*"AI can tell you what the differences are. I guess it could be some
list of the beak is longer for this and that. But I think visually
bringing the differences up side by side, and then I can directly
compare what the differences are."* (P16)

### Preferred explanatory forms {#preferred-explanatory-forms-5 .unnumbered .unnumbered}

[Rule]{style="color: orange"} (12/14) and [counterfactual
example]{style="color: orange"} (10/14) were the most preferable forms.
Participants chose [rule]{style="color: orange"} since *"you could write
that you differentiated the bird's tail were long or short, or beak thin
or thick"* (P10). The [counterfactual examples]{style="color: orange"}
*"identify where specifically to look"* (P16), and*"describe the change,
the progress"* (P11).

[**Learn**]{style="color: blue"}
--------------------------------

Using AI for user's personal learning, improving problem solving skills,
and knowledge discovery, *"depends on how reliable it (AI) really is"*
(P10). And participants expected AI to *"receive human feedback to
correct its error and improve itself"* (P01).

To facilitate learning and knowledge discovery, *"just looking at
(input) pictures and (output) names isn't enough"* (P10), and
participants **expected a wide range of explanations** depending on the
particular learning goal, such as *"more details to systematically
learn, go over that same bird, \...a mind map to build a category of
birds by one feature"* (P02), *"the specific characteristic about this
bird, and how can I differentiate this bird from other birds"* (P04).
Other learning features mentioned by participants include: referring to
external *"respectable source"* (P18), supporting personalized learning
for unfamiliar terms (P04), and *"collecting information about how well
I'm doing on it, like if I guess wrong, does it record that? to see if
I'm progressing"* (P16).

### Preferred explanatory forms {#preferred-explanatory-forms-6 .unnumbered .unnumbered}

Rule-based explanations ([rule]{style="color: orange"}: 12/14, [decision
flow chart]{style="color: orange"}: 10/14, [decision
tree]{style="color: orange"}: 8/14) were more favourable for the need to
learn, since they showed *"a learning process. It has like how you could
recognize a bird. So help me to learn some new knowledge"* (P02). Same
as in [Report]{style="color: blue"}, participants would prefer to see
*"the graphics and text combined"* (P02): *"It combines text and
pictures, and they are relevant to each other. It's kind of a
multi-modal learning"* (P04).

[**Improve the predicted outcome**]{style="color: blue"} {#control}
--------------------------------------------------------

Participants intuitively seek explanations to improve the predicted
outcome, when predictions are related to personal data (in our study,
the House and Health tasks). However, they **tended to unwarrantedly
assume the explanations were causal** (causal illusion [@Matute2015],
i.e., believe there is a causal connection between the breakdown factors
and the outcome), even though the cause-effect relationship has not been
confirmed, and AI largely relies on correlation for
prediction [@Pearl2000]. Only a few participants required more solid
evidence to support the explanations on improving the predicted outcome,
especially when the action was related to critical consequences
(personal health outcomes).

*"I presume the recommendation (on improvement actions from AI) is also
has been backed up by Health Canada, because I think I would tend to
follow the recommendations if I know there's definitely medical support
behind it."* (P24)

*"I would definitely want to know like what can I do to mitigate those
risk factors or to address those things so that I can decrease the risk.
I would really like to know if it had an explanation of how reliable
each source was. Coz I know some studies, they might seem like a
correlation, but it doesn't mean it's a direct cause. So I would really
love it if it could potentially explain how powerful those studies are
suggesting."* (P22)

Regarding the specific requirements on the explanations for improvement,
participants were looking for **controllable features** and ignoring the
features that cannot be changed.

*"I can not change my age, but I'm able to reduce my weights"* (P02).

Knowing the controllable features has a positive psychological effect to
give users a sense of control, and vice versa.

*"If I'm afraid of getting diabetes, and assume that I'm going to
sentence, it feels like there's nothing I can do about it. But when I
see this one ([feature attribute]{style="color: orange"}), I think, 'oh
geez, maybe there are other factors here that I can do something about.'
So this may make me more positive about doing something about my
condition."* (P16)

*"I know it ([feature interaction]{style="color: orange"}) is comparing
my house area and my number of rooms with other houses. I can understand
'okay if I increase my room number, the price will be increased that
much.' But the problem is I cannot change any of them (the house
features). It just gives me the feeling of disappointment."* (P30)

To counterpoise the unchangeable features, users may intuitively apply
counterfactual reasoning to compare different feature adjustment
settings.

*"If I make any change in my house appliance and renew, then I can still
reach the same price as if my house was bigger"* (P30).

*Preferred explanatory forms* [Counterfactual
example]{style="color: orange"} (18/26) and [feature
shape]{style="color: orange"} (13/26) were the top two selected forms.
While [counterfactual example]{style="color: orange"}
(Section [\[ce\]](#ce){reference-type="ref" reference="ce"}) provides
how to achieve the target outcome change by adjusting the input features
(counterfactual reasoning), [feature shape]{style="color: orange"}
(Section [1.2](#fs){reference-type="ref" reference="fs"}) (and [feature
interaction]{style="color: orange"}) allow users to adjust features and
see how that leads to outcome change (transfactual
reasoning [@7933919]).

\centering
![**Clusters of the explanation needs** The explanation needs that are
close to each other indicate they have similar patterns on participants'
explanatory type selection. Specifically, each purpose is represented by
a 12-dimensional vector, where each number in the vector is the total
number of an explanatory type selected for that purpose. We visualize
their relative distances in the 2D scatter plot using PCA dimensional
reduction. explanation needs are marked by different colors indicating
the cluster they belong to using k-means clustering: **Cluster 1**:
Trust, Communication, Unexpected; **Cluster 2**: Safety, Multi-objective
alignment, Bias; **Cluster 3**: Expected, Improvement; **Cluster 4**:
Differentiation, Learning,
Report.](figures/purpose_cluster_2021.pdf){width="50%"}

[\[fig:purpose\_cluster\]]{#fig:purpose_cluster
label="fig:purpose_cluster"}

[**Communicate with stakeholders**]{style="color: blue"} {#communicate}
--------------------------------------------------------

To communicate with other stakeholders, some participants chose to
communicate verbally about their opinions without mentioning AI. Others
preferred to present stakeholders with more evidence by bringing AI's
additional information explicitly to the discussion. For the latter
case, the **other stakeholders need to establish basic understanding and
trust towards AI** before discussing AI's explanations.

*"I'd sit down and get my family together and explain about the
artificial intelligence thing."* (P12, House)

*"I would try to get some evidence from it (AI) that I could take to the
doctor to get them to buy into it."* (P16, Health)

To do so, most participants chose to present AI's performance
information to build trust.

*"As long as the backstage is accurate and then I can just provide
accuracy to my wife and she'll be able to get that. Trustworthy is the
most fundamental."* (P28, House)

Different audiences and explanation needs of communication may require
distinct explanations, as described by P32:

*"I'm pretty sure my husband or my mother has a different way to decide
or they want to know different things"*.

In addition, in the Health task, we asked participants to communicate
with family members or doctors about their diabetes predictions. Since
the requested explanation covered a wide range of contents, we did not
identify any distinct differences in the communicating contents between
the two audiences.

A formal summary or report from AI may facilitate the communication with
other stakeholders, as requested by many participants.

*"A written report from AI that I would be able to reference to, in
order to talk to my family about that. It would feel a little bit more
official rather than just, 'oh, this is what somebody said', there's no
real evidence, whereas this sort of creates that paper trail.''* (P31)

*Preferred explanatory forms* While [output]{style="color: orange"}
(21/46) and [performance]{style="color: orange"} (17/46) provide AI's
result and help to build trust, [feature
attribute]{style="color: orange"} (27/46) and [decision
tree]{style="color: orange"} (17/46) show the breakdown factors and
internal logic behind the prediction.

[**Generate reports**]{style="color: blue"} {#report}
-------------------------------------------

The content of reports may largely depend on the specific purpose and
readers of the report. In our study, participants frequently mentioned
the report should include*"key identifying features"*, *"list of
distinguishing characteristics or what makes it unique"* (P09, P16,
P18), or *"**a summary of factors** that were part of the input led to
the diabetic prediction"* (P31). Users also mentioned including
supporting information to back up the decisions, such as the training
dataset size of the predicted class, and the decision certainty level
(P01).

*Preferred explanatory forms* [Rule]{style="color: orange"}(12/14),
[decision flow chart]{style="color: orange"}(7/14), and [feature
attribute]{style="color: orange"}(5/14) are the most frequently selected
explanatory forms.

Rule descriptions can conveniently generate text reports.

*"I have to write the explanation"* (P08, P09)

*"You can not only by looking at the images and get some explanation.
You need some more specific description."* (P08)

In addition, adding image to the text *"would be complementary"* (P10)
to each other, and the format of image + text were more favourable by
many participants.

*"[Rule]{style="color: orange"} is just describing and writing. It
doesn't really show you a visual on how to compare them."* (P06)

*"[Feature attribute]{style="color: orange"} and [decision flow
chart]{style="color: orange"} (presented in image format on bird
recognition task) highlights what [rule]{style="color: orange"} is
saying, this knowledge complements your statement."* (P10)

[**Trade-off multiple objectives**]{style="color: blue"} {#multi}
--------------------------------------------------------

Usually it is the human user rather than AI to trade-off among multiple
objectives in AI-assisted decision-making tasks. Thus when multiple
objectives get conflicted (in our study, they are scenarios when car
drives autonomously and passenger gets a car sick; and AI predicts
diabetes and uses it to determine insurance premium), AI was required to
allow users to take over or to receive users' inputs.

*"It's the most important thing I would want to do is to allow me to
stop, or asking to slow down if I'm feeling sick."* (P03, Car)

Explanations are required if the multiple objectives conflict and need
to trade-off. And users could use such explanations to defend for or
against certain objectives.

*"I think it's like a defensive thing, like if I'm expecting that
they're going to cause an increase in my payments or whatever they're
going to deny me (health insurance) coverage, I would be trying to find
out what it's based on for the opposite reason maybe to discredit it."*
(P16, Health)

Discussions {#disussion}
===========

We state how the EUCA framework supports HCI/AI practitioners and
researchers to build end-user-oriented XAI systems/algorithms, and
discuss our findings and compare them with prior literature.

Utilities of the EUCA Framework
-------------------------------

### **Explanatory Forms as Building Blocks** {#practitioner}

In the user study, participants sorted the explanatory form prototyping
cards, and combined them to construct a low-fidelity prototype.
Participants rated the resulting prototype fulfilled majority of
explanation needs (231 out of 279 responses, 83%). This shows that the
explanatory forms in the EUCA framework may serve as building blocks
that can be combined to complete an explanation. The finding resonates
with previous user studies that an XAI system should support
"integrating multiple explanations", as "users employed a diverse range
of explanations to reason variedly" [@Wang2019]. The combination helps
to overcome the weakness of an individual explanatory form, and may make
the explanation more robust, complete, and versatile. With multiple
explanatory forms that complement each other, users may construct a
whole picture about AI's decision process more easily, and may mitigate
confirmation bias, attribution bias, and anchoring
bias [@Lighthall2015a].

Different explanatory forms can be combined *statically* as different
modules in the UI, or *interactively* combined and incorporated in the
UX to show detailed explanatory forms
on-demand [@Sokol2020; @Cheng2019; @Smith-Renner2020a]. The contents of
combination can be *fixed* or *dynamically* generated, i.e., the XAI
system learns to use different explanatory forms as vocabularies to
respond to user's follow up questions, so that to construct an
interactive explanatory conversation [@Weld2018] with end-users.

### **Suggested Prototyping Process**

Our user study demonstrated the prototyping and co-design process with
end-users. To determine the most feasible combination of the explanatory
forms to construct prototypes for a particular XAI system, we summarize
the prototyping process from our user study, and suggest the following
co-design and prototyping workflow.

\centering
![**Suggested Prototyping Workflow using EUCA Framework** Blue bold text
highlights the supporting contents provided by
EUCA.[]{label="fig:workflow"}](figures/euca_workflow.pdf){#fig:workflow
width="\textwidth"}

1.  **Create prototyping cards from explanatory forms**

    The designer starts by **manually extracting several interpretable
    features** given the AI task and input/output data type. For
    example, for tabular data, the features could be the column names
    that describing the input, such as house size, age, and location.
    For image data, the features could be saliency image part or object
    for recognition, such as cars, traffic signs, or pathological
    appearance of a disease on chest X-ray. As quick prototyping, the
    feature content may not necessarily reflect the true content
    generated by XAI algorithms. They served as content placeholders for
    the prototyping card design template.

    Then the designer can use the prototyping card design template
    provided by EUCA, and **fill in the template with the above
    extracted features**. In the design template and example, we provide
    the basic visualization of the explanatory forms used in the user
    study. Designers can also create their own template from scratch by
    referring to the design examples. The EUCA framework website[^2]
    supports designers sharing of their prototype design to expand the
    available design templates, and to encourage the reuse of design
    patterns on similar XAI applications.

    For a particular explanatory form, the designer may **prepare
    multiple versions varying the visual representations** (e.g.:
    graphics or text) and UI layout, alternating contents from brief to
    details, and providing different options, such as whether to use
    pre-defined or user-defined contrastive outcome on [counterfactual
    example]{style="color: orange"}, whether to give users the option to
    set a threshold level for [feature
    attribute]{style="color: orange"}, or refer to the UI/UX design
    implications part in the user study findings
    (Section [1](#rq22){reference-type="ref" reference="rq22"}). Each
    explanatory form and its variations are presented on individual
    prototyping cards.

    While designing UI/UX variations for the prototyping cards,
    designers may also consider and **apply the general human-AI
    interaction guidelines**. We selected the following design
    guidelines that are more relevant to XAI system: "remember recent
    interactions", "support efficient invocation, dismissal and
    correction", "remember recent interactions", "learn from user
    behavior", and "encourage granular feedback". Designers can refer to
    the guideline paper [@Amershi] for details.

2.  **Co-design and iterate low-fidelity prototype with end-users** With
    the prepared prototyping cards, the designers then can meet and
    discuss with the target end-users and/or other stakeholders of the
    XAI system, and apply user-centered methods informally or formally.
    Such methods may include interview, focus group, and card sorting.
    The communication aims to use the created cards as a prototyping
    tool to understand users' needs under potential explanation needs,
    and involve end-users in the co-design and prototype iteration
    process.

    To quickly create a low-fidelity paper prototype from the
    prototyping cards, the **end-users can select, rank, combine, modify
    the prototyping cards**, and sketch new ones. In this process,
    designers may ask users why they selected or did not select a card,
    and their rationals for making such a combination, whether the
    combination could fulfill their requirements, and what is lacking in
    the current prototype. The users can easily manipulating the card
    positions to try out different layouts to examine different UI
    design possibilities (for example, on brewers, tablet or mobile
    phone).

    Users can also comment on and revise each variation of the same
    explanatory form. With the tangible prototyping card examples,
    designers can know in-details about users specific requirements on
    the UI/UX design. The prototyping cards may facilitate the
    discussion of UX design, for examples, users may choose to hide some
    cards and only show them on-demand, or to present different
    explanatory information in different contexts.

    After the initial communication with users, designers need to
    synthesize users comments and decide one or several prototype
    designs (such as using majority voting). Then based on the
    prototyping card ranking and combination, the designer may create
    low-fidelity prototypes, and continue to seek user and/or other
    stakeholders' feedback and iterate the prototype.

    During the above process, the designer may refer to the user study
    findings to be informed about the properties of the explanation
    forms (pros, cons, applicable explanation needs, and design
    implications in Section [1](#rq22){reference-type="ref"
    reference="rq22"}), and to understand end-users' diverse explanation
    needs (to calibrate trust, detect bias, resolve disagreement with
    AI, etc. in Section [2](#rq12){reference-type="ref"
    reference="rq12"}).

3.  **Implement functional prototype**

    After co-design and several iteration, when the low-fidelity
    prototype is ready to implement, given that many existing XAI
    techniques are implemented as open-source toolkits
    (e.g.: [@alibi; @DALEX; @iml; @Arya2019; @lime; @Captum]), the
    development team can identify the most viable technical solution
    according to the corresponding XAI algorithms
    (Table [\[framework\]](#framework){reference-type="ref"
    reference="framework"}) of the selected explanatory forms in
    low-fidelity prototypes.

### **Insights for novel XAI algorithms/interfaces** {#researcher}

Our findings provide design implications and insights from end-users'
perspectives. It would motivate HCI and AI researchers to develop novel
interfaces/algorithms towards end-user-centered XAI. We give some
examples for inspiration:

-   The design implication in [similar example]{style="color: orange"}
    (Section [1.4](#se){reference-type="ref" reference="se"}) indicates
    users need to pinpoint the corresponding features among similar
    examples for easy comparison. This requirement can be regarded as a
    combination of the two explanatory forms [similar
    example]{style="color: orange"} and [feature
    attribute]{style="color: orange"}. Such insight may inspire UX
    researchers to design novel interfaces to support highlighting and
    comparing important features among instances on tabular data.
    However, this novel XAI interface is not applicable for image data,
    and new XAI algorithms need to be proposed, such
    as [@Chen; @Codella2018a].

-   Participants suggested to click features in [feature
    attribute]{style="color: orange"} to check details of [feature
    shape]{style="color: orange"}. It can be regarded as a combination
    of the two explanatory forms. Such a combination can be achieved at
    the interface level, e.g.: Gamut [@Hohman2019], or at the
    algorithmic level, e.g.: COGAM [@Abdul2020].

-   The advantages and disadvantages of [similar
    example]{style="color: orange"} and [typical
    example]{style="color: orange"} seem to be complementary to each
    other. A new type of example-based explanation may be proposed
    accordingly: it creates typical examples that are representative to
    the target class, while being as similar as possible to the input
    instance. Thus by taking the advantage of [similar
    example]{style="color: orange"}, it is similar to the input instance
    to be easily understood, thus overcomes the disadvantage of [typical
    example]{style="color: orange"} for being unrelated to the input
    instance; meanwhile it inherents the advantage of [typical
    example]{style="color: orange"} for being distinct and not
    confusing.

The above examples demonstrate using the explanatory forms as building
blocks to create novel XAI algorithms/interfaces. In addition to the
identified design implications in our study, XAI researchers can use the
above prototyping method to identify users' requirements in their
particular tasks, and propose new interfaces or algorithmic solutions
accordingly.

Since explanation is a social process [@Miller2017], an advanced XAI
system may be trained to construct an explanation dialog [@Weld2018]
that mimics the human explanation process. New XAI algorithms can also
be created in line with such a manner, for example, by using
reinforcement learning to use different explanatory forms to respond to
the user's current query and make such explanations adapted to users'
preferences or explanation needs.

End-Users' Explanation Needs {#need_discuss}
----------------------------

XAI techniques are abundant, but understanding on end-users' needs is
little. In this section, we present the user study findings on
end-users' diverse needs for explainability within the context of
explanatory forms. Our findings reveal two major themes of the need for
explainability: explanations for verification/justification, and
explanations for betterment.

###  "How do I know when my prediction is not an error?'': End-users' verification of decision quality {#justify_discuss}

After acknowledging AI's decision is probabilistic, most users need
explanations for decision verification, so that they could incorporate
AI into their own decision process on high-stake tasks. In our study, we
discovered users frequently seek decision quality metrics, followed by
explanations answering *why* or *how* questions (such as [feature
attribute]{style="color: orange"} and [similar
example]{style="color: orange"}) to verify the decisions. Users usually
request such information **1**) during the initial deployment
stage [@Liao2020] when [trust]{style="color: blue"} has not been
established so that users do not have knowledge on the observed
performance [@Yin2019], as in the explanation needs of
[safety]{style="color: blue"} and [communicate]{style="color: blue"};
and **2**) when AI's decision is being challenged, as in the explanation
needs of [bias]{style="color: blue"} and
[unexpected]{style="color: blue"}. Our quantitative results also
revealed that the decision quality-related metrics
([output]{style="color: orange"}, [performance]{style="color: orange"},
and [dataset]{style="color: orange"}) were frequently selected and
ranked higher for the above explanation needs
(Fig. [\[fig:mtx\]](#fig:mtx){reference-type="ref"
reference="fig:mtx"}).

In our study, we found that most participants accepted and understood
the decision certainty in [output]{style="color: orange"}, followed by
[performance]{style="color: orange"}. The training data distribution in
a [dataset]{style="color: orange"} was the least comprehensible form.
Interpreting these metrics may require a certain degree of data analytic
skills and could be time-consuming. The numbers may be contradicting and
cause users' frustration. Thus, in real-world applications, it may not
be feasible for end-users to check all the metrics. To indicate the
probabilistic nature of AI, our findings
(Section [1.10](#output){reference-type="ref" reference="output"})
suggest a possible workaround is to provide the range of prediction
on-demand or a point prediction within its range. The range may bring
additional benefits of leaving rooms for flexible and negotiable
decisions for specific tasks. Another suggestion is to provide a unified
and precise uncertainty estimation [@Begoli2019b] metric that is case
specific, incorporating all sources of decision uncertainty (such as
performance on model capabilities, prior knowledge about the training
data distribution, noises on input data, etc), to indicate the
capabilities and limitations of AI prediction.

Alongside the above metrics, various other explanatory forms were
selected by participants to verify AI's decision
([trust]{style="color: blue"}, [safety]{style="color: blue"},
[bias]{style="color: blue"}, [unexpected]{style="color: blue"}). The
selection of explanatory forms largely depends on the specific task, the
explanation need, and users' preferences, and there are no definite
patterns. Previous quantitative results showed discrepancies of
providing local explanations ([feature attribute]{style="color: orange"}
or [similar example]{style="color: orange"}) and its effect on trust
calibration and users' decision accuracy [@Lai2019; @Zhang2020],
indicating explanations may play a complex role in the AI-assisted
decision process. It may involve complex interactions among factors such
as users' perception of the explanatory forms and their visual
representations/layouts, AI and human's different error
zones [@Zhang2020], explanatory information overload, users' cognitive
bias when interpreting the explanations [@Lighthall2015a], and how
faithful the explanations are to the underlying AI model, etc. Future
research is needed to explore these factors and their effects on
human-AI collaborative decision quality. Because there lacks a universal
model to predict various explanatory forms and their outcomes, our
proposed EUCA framework could serve as a practical prototyping tool to
quickly test the effects of various explanatory forms to guide the
design process.

### Explanations for betterment {#improve_discuss}

The other major motivation to check AI's explanation is to move beyond
decision verification, and to improve users' current status, such as to
[improve]{style="color: blue"} the predicted outcome, enhance users'
[learning]{style="color: blue"} and problem-solving skills, discover new
knowledge, and trade-off among [multiple
objectives]{style="color: blue"}. Those explanation needs may emerge as
users established trust and adopted AI into their decision workflow. As
AI surpasses human performance in some critical tasks, AI can act as a
knowledgeable source providing insights for humans to improve their own
welfare. Although research in this direction is relatively limited, some
prior works provide promising results on using machine explanations to
improve users' knowledge and task performance [@Aodha2018; @Lai2020].

Limitations and future work {#limitation}
===========================

The limitations and future work include:

-   We summarized the end-user-friendly explanatory forms from
    technically-achievable solutions via a literature/critical review.
    We aimed to include the majority of existing explanatory forms with
    the information saturation criterion: i.e. no more additional
    explanatory forms could be identified. This process manifested in a
    conceptual model of the 12 end-user-friendly explanatory forms that
    served as a starting point for subsequent user study [@review]. We
    did not aim to conduct an exhaustive, comprehensive systematic
    review, which is beyond what one paper could achieve. And since XAI
    techniques are fast evolving, the current framework may not
    necessarily cover all possible algorithms. The EUCA framework aims
    to serve as a moderate initial step towards a practical
    end-user-centered XAI framework, and is extendable to update with
    any emerging XAI technologies on the EUCA website[^3].

-   Due to the high-stake nature and limited adoption of AI in critical
    decision-support, it is challenging to gain access to real-world AI
    systems in high-stake facilities (such as police offices, courts,
    clinics/hospitals, banks) to conduct user studies on multiple
    critical tasks, and recruit domain-specific end-users (such as
    physicians, police officers, judges, bankers). This is beyond the
    scope of one single paper could achieve. Therefore in the user
    study, we designed four fictional vignettes to represent the
    variability of AI-supported critical decision-making tasks, and
    participants' responses were based on conjecture rather than their
    real experience with AI. Our ongoing future work on XAI system
    design involves physicians as domain expert end-users using AI as
    support in their day-to-day clinical decision tasks. Future work may
    apply the EUCA framework in other domain-specific XAI design and
    development practices to iterate and improve the framework.

-   Bias may be involved in the card sorting of explanatory forms, as we
    noticed a few participants selected a card because it contained
    certain features rather than its distinguished form, despite in the
    follow-up questions we asked "what if the specific feature was or
    wasn't included". The explanatory forms, their contents, the
    particular visual representations, the task, user's current
    explanation needs, and user type all played a role in participants'
    selection choices under the specific study context, and our study
    design could not disentangle them. The quantitative results from
    card sorting are meant to serve as a reference only. They are not
    meant to be used directly to choose explanatory forms without the
    prototyping process, due to the above complex factors involved.
    Future work may design randomized controlled user studies to
    quantitatively examine the effects of the above factors in detail to
    guide the choice of explanatory forms in specific contexts. The EUCA
    framework website allows community users to share their prototypes,
    encouraging the reuse of design patterns on certain XAI
    applications.

Conclusion
==========

Designing end-user-oriented explainable AI systems faces many
challenges. From the user side, **1**) End-users have diverse roles,
tasks, and explanation needs. **2**) End-users lack technological
knowledge which is a prerequisite for some XAI systems in order to
interpret the explanation. From the XAI practitioner side, **3**)
practitioners' expertise on AI or HCI/UXUI design usually does not
overlap, and there lacks boundary objects to connect the two fields and
facilitate collaboration between AI and HCI practitioners. **4**) there
lacks tools to support UI/UX design, prototyping, and co-design process.

To address the above challenges, we developed the end-user-oriented XAI
framework EUCA with a collaborative effort of combining AI and HCI
expertise. EUCA considers not only the human-centered perspective but
also the technological capabilities, so that the design solutions are
both end-user-oriented and technically achievable. It acts as a boundary
object between AI and HCI filed and provides UI/UX design, prototyping,
and co-design support.

To apply EUCA in practice, XAI designers can use the provided design
templates to create prototyping cards for the twelve explanatory forms.
The explanatory forms are end-user-friendly and were identified from
technically achievable solution space. They are a familiar and mutual
language to both end-users and XAI practitioners. With the prototyping
cards, designers can conduct a participatory design process that
involves multiple stakeholders to receive their feedback and iterate the
prototype. In this process, the stakeholders can comment, sort, combine,
and revise the prototyping cards, to use them as building blocks to
build a low-fielty prototype. Designers can also refer to the user study
findings to be informed by end-users about the properties of the
explanation forms (their strength, weakness, UI/UX design implications,
and applicable explanation needs), and to understand end-users' diverse
needs for explainability within the context of explanatory forms. The
corresponding XAI algorithms for each explanatory form can facilitate
developers to implement a functional prototype. As an initial step
towards end-user-centered XAI, the EUCA framework provides a practical
prototyping toolkit that supports HCI/AI practitioners and researchers
to develop end-user-oriented XAI systems.

[^1]: Although the AI community has distinct methods to compute output
    likelihood and uncertainty level, in our study we used likelihood,
    confidence and uncertainty interchangeably to avoid participants'
    confusion.

[^2]: http://weina.me/end-user-xai

[^3]: http://weina.me/end-user-xai
