# Week 13 Reflection
## Data Source

ChatGraph: Chat with Your Graphs

Yun Peng, Sen Lin, Qian Chen, Lyu Xu, Xiaojun Ren, Yafei Li, Jianliang Xu

https://arxiv.org/pdf/2401.12672

## Reflection
For my final reflection, I focused on ChatGraph -- a tool similar yet distinct from our final project that calls APIs specific to a user's query about graph questions.
Like us, they use an LLM, but rather than using tools they have different API interpreting pipelines depending on a type of graph:

![image](https://github.com/akerekon/reflections-research/assets/89589162/42e4b17f-d71e-42f8-a248-237cf1374d0f)

They fine-tune this API in chains to prevent losing content and always have the right sense of how to interpret data. The image below shows how they interpret a 3D graph based on a 2D image using a specific call:

![image](https://github.com/akerekon/reflections-research/assets/89589162/faf854e7-a2e1-4865-af9e-b9529ebe4109)

They do this via approximate-nearest-neighbor (ANN) to find the right tool for the job, including tools to summarize and retrieve data from pure text itself. They are even able to modify the API-chain of calls based on prompting the included LLM chatbot with questions!

![image](https://github.com/akerekon/reflections-research/assets/89589162/a9ece311-b4c5-466e-bdcd-c55f9faa4835)

Despite this, they do not include a table of results, and their demo is only four pages. I'm exicted to see future work and I'm hopeful our project can expand on projects like these!



