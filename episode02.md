---
title: "Introduction to AI and Machine Learning for GLAM"
teaching: 10
exercises: 5
questions:
- "What are Artificial Intelligence (AI) and Machine Learning (ML)?"
objectives:
- "Understand Machine Learning as a subfield of AI and name two others"
- "Name four types and machine learning and describe the difference between supervised and unsupervised learning"
- "Describe the difference between a model of data, and a model trained on data"


keypoints:
- "Machine Learning is a subfield of AI which identifies patterns in data"
- "Supervised learning algorithms learn by example"
- "Unsupervised learning algorithms put data into groups of similar objects or records"
---

## What is the difference between Machine Learning and AI?

The field of Artificial Intelligence has been around since the 1950s (ref: Dartmouth Conference). It is a broad topic which encompasses a number of sub-fields including but not limited to: Logic, Probability, Knowledge Representation, and Machine Learning.

Figure 1 shows how a system based on Artificial Intelligence might function:

![Alt text](https://g.gravizo.com/source/custom_mark10?https%3A%2F%2Fraw.githubusercontent.com%2Fmark-bell-tna%2FMachineLearningCourse%2Fmaster%2Fepisode02.md)
<details> 
<summary></summary>
custom_mark10
  digraph G {
    size ="4,4";
    main [shape=box];
    main -> parse [weight=8];
    parse -> execute;
    main -> init [style=dotted];
    main -> cleanup;
    execute -> { make_string; printf};
    init -> make_string;
    edge [color=red];
    main -> printf [style=bold,label="100 times"];
    make_string [label="make a string"];
    node [shape=box,style=filled,color=".7 .3 1.0"];
    execute -> compare;
  }
custom_mark10
</details>

The history of Logic stretches all the way back to Aristotle in the Organon and was formalised by George Boole in the 19th century (hence the name Boolean Logic). With logic we can write rules to reason about data or make decisions. “If it rains I will carry an umbrella”.
Logical rules are based on things being True or False but the world is not so clear cut. Probability lets us add doubt and uncertainty: “It might rain today, should I take an umbrella?”.
With logical rules and probability we can solve quite complex tasks, but there are limits: “Which paintings in our collection have umbrellas in them?”.
