# Week 11 Reflection
## Data Source
Xuan Long Do, Mohammad Hassanpour, Ahmed Masry, Parsa Kavehzadeh, Enamul Hoque, and Shafiq Joty

Do LLMs Work on Charts? Designing Few-Shot Prompts for Chart Question Answering and Summarization

https://arxiv.org/pdf/2312.10610.pdf

## Reflection
For my reflection, I wanted to continue to focus on Charts as they related to Large Language Models, which is the focus of my group's final project. This team's approach, PromptChart, is particularly interesting as they propose a few-shot prompting model that is able to gracefully handle unseen input, as compared to previous fine-tuned pretrained models that do not perform well upon seeing data unfamiliar to their training set. 

The real benefit, in addition to being able to handle unknown data, is taking far less computational resources -- training and fine-tuning is expensive not only during training, but also in the massive scope of high-quality training data required. This also allows for "LLM-as-a-service" that can be hosted without needing a wide array of resources.

The team proposes the following model to realize their vision:
![image](https://github.com/akerekon/reflections-research/assets/89589162/667073e4-2620-41e0-b0e4-434e914c3b26)

The beauty of this model is it relies on an included "Visual Data Table Generator" that interprets charts as data tables, which then are piped into each prompt specified by the user. In that fashion, the LLM model can rely on data from the chart that has already been preprocessed into a format it can understand. 
This allows the team to answer three key types of questions:
1. Factoid (simple, fact-based question to elicit brief factual response)
2. Chart summarization
3. Long-form question (abstract, open-ended paragraph response)

![image](https://github.com/akerekon/reflections-research/assets/89589162/1d362e68-d39f-454f-bb90-a72167c3ee03)

While output often isn't perfect, it gets relatively close to many answers, and future work can be performed to prevent any potential hallucinations or misinterpretations of passed data.
