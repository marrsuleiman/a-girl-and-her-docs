---
layout: page
title: Explainability
permalink: /Explainability/
---

This section covers the concept of explainability in machine learning, its importance, and how Seldon Deploy applies explainability.

- [Explanablity](#explanablity)
  - [Why is Explainability important?](#why-is-explainability-important)
    - [Explanablilty with Alibi Explain](#explanablilty-with-alibi-explain)

 
# Explanablity
Explainability is a term in machine learning that describes how a model arrives at a decision or prediction. Data scientists can apply the principle of explainability through the use of explainers like [Seldon's Alibi Explain](https://docs.seldon.io/projects/alibi/en/latest/index.html " An open-source Python library aimed at machine learning model inspection and interpretation"). By introducing explainer models as part of their process, data scientists can increase transparency and support stakeholders in understanding how machine learning systems make predictions.

## Why is Explainability important?
Explainability facilitates the ability to [audit and trace](https://ec.europa.eu/futurium/en/ai-alliance-consultation.1.html "Building trust in human-centric AI") how a model arrived at a prediction. Building trust in the process, and prompting reconsideration in sensitive cases where variables such as gender, class, and age can affect the outcome of a prediction of whether an individual will be successful in a loan application.

As machine learning has evolved, regulations to protect people have followed. With article 14 of the General Data Protection Regulation, organizations and data scientists must make individuals aware of automated processes and how the processes arrive at a decision. The practice of using [Alibi Explain](https://docs.seldon.io/projects/alibi/en/latest/examples/overview.html "Alibi Overview Example") comes not only from an ethical perspective but a legal one.

### Explanablilty with Alibi Explain
Models can either be [black-box or white-box models](https://docs.seldon.io/projects/alibi/en/latest/overview/white_box_black_box.html "Black box and White box models descriptions"). The algorithm of a white-box model can be explained because it is possible to trace the variables that led to a prediction. For example, in a linear regression model where it is easy to discern how the independent variables led to the prediction of the dependent variable.

Although black-box models such as deep neural networks are powerful, *how* these models make a prediction is impossible for a data scientist to investigate because the algorithms could be behind an API endpoint. With the results of a black-box model alone, clinicians, for example, will not be able to justify their recommended treatment plan if the data scientists they work with cannot demonstrate how the model arrived at the prediction. The ability to understand a prediction is where methods like [**Anchor**](https://docs.seldon.io/projects/alibi/en/stable/methods/Anchors.html) in Alibi Explain can be utilized to demonstrate why the model arrived at the prediction.

Take a method like [**Counterfactuals with Reinforcement Learning**](https://docs.seldon.io/projects/alibi/en/stable/methods/CFRL.html#Overview "aka counterfactual instances") and the scenario of the clinician with a high-risk patient. Counterfactual explanations can be used to gain insight into which health factor (weight, sugar consumption) needs to be addressed to reduce disease risk. Using a counterfactual explanation can point the clinician to the changes in lifestyle that the patient would have to make to prevent the patient from getting the disease.
