## Project title: "Toxic Comment Classification using Label Studio"

For this project the dataset was selected from the Kaggle website (https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data). The data contains information about a large number of Wikipedia comments which have been labeled by human raters for toxic behavior. The dataset has 159403 lines, for this project I took a small portion of it (200 tasks).

1) Annotation goal: Classify the comments into different types of toxicity such as toxic, severe toxic,obscene, threat, insult, identity hate, or clean.

2) Tools used: I used Python for the cleaning process of the dataset and the creation of the json file. On the other hand, Label Studio was the tool I used for the annotation process

3) Label Studio Configuration
```xml
<View>
  <Header value="Toxic Comment Labeling"/>
  <Text name="text" value="$text"/>
  <Choices name="toxicity" toName="text" choice="multiple" required="true">
    <Choice value="Toxic"/>
    <Choice value="Severe Toxic"/>
    <Choice value="Obscene"/>
    <Choice value="Threat"/>
    <Choice value="Insult"/>
    <Choice value="Identity Hate"/>
    <Choice value="Clean"/>
  </Choices>
</View>

