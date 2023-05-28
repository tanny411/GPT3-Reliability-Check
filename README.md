## Reliability Check: An Analysis of GPT-3’s Response to Sensitive Topics and Prompt Wording
Authors: Aisha Khatun, Dan Brown
Affiliation: David R. Cheriton School of Computer Science, University of Waterloo, Canada.
Publishing Venue: TrustNLP Workshop, ACL 2023.

### Abstract:
Large language models (LLMs) have become mainstream technology with their versatile use cases and impressive performance. Despite the countless out-of-the-box applications, LLMs are still not reliable. A lot of work is being done to improve the factual accuracy, consistency, and ethical standards of these models through fine-tuning, prompting, and Reinforcement Learning with Human Feedback (RLHF), but no systematic analysis of the responses of these models to different categories of statements, or on their potential vulnerabilities to simple prompting changes is available. In this work, we analyze what confuses GPT-3: how the model responds to certain sensitive topics and what effects the prompt wording has on the model response. We find that GPT-3 correctly disagrees with obvious Conspiracies and Stereotypes but makes mistakes with common Misconceptions and Controversies. The model responses are inconsistent across prompts and settings, highlighting GPT-3's unreliability.

### Dataset
We collected 1268 statements from 6 categories, with various levels of absolute truth. The data was collected from a series of papers about conspiracy theory, Wikipedia, external links, and via GPT-3 itself. The source of each data point is provided with the dataset. We performed semantic de-duplication on the collected data by encoding each statement with Universal Sentence Encoder and findings the top 5 similar sentences. 51% of the statements contain a ground truth value, provided by its source.

The dataset is available [`here`](data/data.csv).

### Code

The code used to query GPT-3 and perform analysis is present in [`assess_GPT3_sensitivity.ipynb`](assess_GPT3_sensitivity.ipynb) notebook. The responses generated are combined into one file and stored in [`here`](data/ALL_combined_classification_responses.csv).

### Citation

If you use our dataset, please cite using the following citation:
```
```
