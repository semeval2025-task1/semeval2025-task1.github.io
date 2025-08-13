---
title: SemEval-2025 Task 1 - Test / Evaluation Data
---

Test datasets are to be used for final system performance evaluation and competition ranking on the CodaBench platform during the evaluation phase.

Note that labels are not supplied for the test data; output scoring should be done using the CodaBench platform.

Labelled versions of the evaluation datasets may be obtained from the [ORDA repository](https://doi.org/10.15131/shef.data.28436600). Note that the **sentence_type** and **expected_order** fields should not be consumed by systems and are made available for analysis purposes.

**Update 2025-01-20:** We have released extended evaluation sets for each language. The compounds used in these sets overlap with the training, development and test sets but they feature different context sentences in which the compounds appear. The increased evaluation set size will hopefully enable more robust assessment of model performance.

Note that the extended evaluation sets exist *in addition to* the primary test sets.



### Data Description

The development datasets contain the folllowing files:

## Subtask A

AdMIRe Subtask A Test.zip

English evaluation data for Subtask A.

15 items.

See the [Training Data page](/data/training/training_data.md) for a detailed description.
Note that the fields **sentence_type** and **expected_order** should be treated as blank for evaluation, with the latter being the target output.

AdMIRe Subtask A Extended Evaluation.zip

English extended evaluation data for Subtask A.

100 items.


AdMIRe Subtask A PT Test.zip

Brazilian Portuguese evaluation data for Subtask A.

13 items.

See the [Training Data page](/data/training/training_data.md) for a detailed description.
Note that the fields **sentence_type** and **expected_order** should be treated as blank for evaluation, with the latter being the target output.

AdMIRe Subtask A PT Extended Evaluation.zip

Brazilian Portuguese evaluation data for Subtask A.

55 items.

## Subtask B

AdMIRe Subtask B Test.zip

English training data for Subtask B.

5 items.

See the [Training Data page](/data/training/training_data.md) for a detailed description.
Note that the fields **sentence_type** and **expected_order** should be treated as blank for evaluation, and are the target output for systems.


AdMIRe Subtask B Extended Evaluation.zip

English training data for Subtask B.

30 items.
