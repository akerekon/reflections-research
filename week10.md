# Week 10 Reflection
## Data Source
Yuan Tian, Weiwei Cui, Dazhen Deng, Xinjing Yi, Yurun Yang, Haidong Zhang, Yingcai Wu

ChartGPT: Leveraging LLMs to Generate Charts from Abstract Natural Language

https://ieeexplore.ieee.org/abstract/document/10443572 (WPI login required for full document)

## Reflection
For my reflection this week, I wanted to close-read a research paper relating to my final project, a portion of which relates to generating charts using LLM prompts. 
I landed on ChartGPT, which addresses the well-known flaws in LLM hallucination through the use of step-by-step fine-tuned prompting, all verified through user input and use of a user study. 

The main takeaways of this research were to...
1. Create a framework to generate charts from LLMs
2. Construct a dataset of charts generated from particular phrases for future research
3. Conduct user studies on the impact of these visualizations

The most important takeaway as it relates to our research is the ability to interpret which type of chart might fit a particular dataset/prompt best. As we aim to allow users to switch between chart types, this will allow our model to provide suggestions to the end user based on the shape of their data. By selecting and choosing various data channels across many domains, we can utilize these findings to model how our own application might be able to generate similar charts after having read user data. 

![Data Pipeline](https://github.com/akerekon/reflections-research/assets/89589162/9b23e62a-dade-4a10-a311-f7310ba00542)

Data Pipeline

![User Selection of Best Chart Type](https://github.com/akerekon/reflections-research/assets/89589162/04f3a960-8b83-4348-a26c-b59ef9f9e71d)

User Selection of Best Chart Type

![Performance](https://github.com/akerekon/reflections-research/assets/89589162/fa460332-56e8-4fcd-9783-cd30a671034c)

Ultimately, their model (as ranked by 12 participants) far outperformed existing work for which graphs were of the best type, after having been trained on how to use the application.
