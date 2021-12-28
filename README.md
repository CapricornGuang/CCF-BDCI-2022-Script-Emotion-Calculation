# Aspect based Emotion Analysis

## Data

The data comes from the CCF competition [爱奇艺剧本情感识别](https://www.datafountain.cn/competitions/518). 

## Thought

Aspect based emotion analysis is a rather complex task. In this competition, We transform this task to a Question-Answer problem. The material is the sentences and the question "What's the emotion of XXX"

## Our Model

We only use RoBerta Chinese pre-trained language model, and add six regression layers for different emotions.<Happy, Angry, Sadness, Threat, Love, Afraid>. 

We strongly recommend you don't modify the model itself unless you have enough confidence. 

## Input Type

[CLS]+text+[SEP]+Aspect+[SEP]

text: we will combine the context of the same scene together

aspect: it's a question-like sentence.

## Result

We only train for one epoch, and get 0.7+ scores. If anyone consider using our code, you may get better result!

