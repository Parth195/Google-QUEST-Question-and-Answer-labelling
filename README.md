# Google-QUEST-Question-and-Answer-labelling



## **Description**

Computers are really good at answering questions with single, verifiable answers. But, humans are often still better at answering questions about opinions, recommendations, or personal experiences.

Humans are better at addressing subjective questions that require a deeper, multidimensional understanding of context - something computers aren't trained to do well…yet.. Questions can take many forms - some have multi-sentence elaborations, others may be simple curiosity or a fully developed problem. They can have multiple intents, or seek advice and opinions. Some may be helpful and others interesting. Some are simple right or wrong.


![image](https://github.com/Parth195/Google-QUEST-Question-and-Answer-labelling/assets/89126978/acfad4b6-683e-46cb-809c-f5a8a856283a)


Unfortunately, it’s hard to build better subjective question-answering algorithms because of a lack of data and predictive models. That’s why the CrowdSource team at Google Research, a group dedicated to advancing NLP and other types of ML science via crowdsourcing, has collected data on a number of these quality scoring aspects.

In this competition, you’re challenged to use this new dataset to build predictive algorithms for different subjective aspects of question-answering. The question-answer pairs were gathered from nearly 70 different websites, in a "common-sense" fashion. Our raters received minimal guidance and training, and relied largely on their subjective interpretation of the prompts. As such, each prompt was crafted in the most intuitive fashion so that raters could simply use their common-sense to complete the task. By lessening our dependency on complicated and opaque rating guidelines, we hope to increase the re-use value of this data set. What you see is what you get!

Demonstrating these subjective labels can be predicted reliably can shine a new light on this research area. Results from this competition will inform the way future intelligent Q&A systems will get built, hopefully contributing to them becoming more human-like.



## **Evaluation**


Submissions are evaluated on the mean column-wise Spearman's correlation coefficient. The Spearman's rank correlation is computed for each target column, and the mean of these values is calculated for the submission score.

## **Submission File**
For each qa_id in the test set, you must predict a probability for each target variable. The predictions should be in the range [0,1]. The file should contain a header and have the following format:

qa_id,question_asker_intent_understanding,...,answer_well_written
6,0.0,...,0.5
8,0.5,...,0.1
18,1.0,...,0.0
etc.



## #**Notebooks Requirements**

Kerneler

This is a Notebook-only competition
Submissions to this competition must be made through Notebooks. Your Notebook will re-run automatically against an unseen test set, and needs to output a file named submission.csv. You can still train a model offline, upload it as a dataset, and use the notebook exclusively to perform inference.

In order for the "Submit to Competition" button to be active after a commit, the following conditions must be met:

CPU Notebooks <= 9 hours run-time
GPU Notebooks <= 2 hours run-time
Internet must be turned off
In synchronous Notebooks-only competitions, note that a submission that results in an error--either within the notebook or within the process of scoring--will count against your daily submission limit and will not return the specific error message. This is to limit probing the private test set.

Please note - committing your Notebook will result in a full execution of your code from top-to-bottom.

Please see the Code Competition FAQ for more information on how to submit.
