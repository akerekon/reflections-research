# Week 12 Reflection
## Data Source

ChartLlama: A Multimodal LLM for Chart Understanding and Generation

Yucheng Han, Chi Zhang, Xin Chen, Xu Yang, Zhibin Wang, Gang Yu, Bin Fu2, Hanwang Zhang

https://arxiv.org/pdf/2311.16483.pdf

## Reflection
This week, I took a detour back to do a deeper dive into a paper I had read several weeks back for my final project -- ChartLlama. This paper caught my attention specifically for its chart extraction, chart-to-chart, and text-to-chart capabilities that we would incorporate into our work:

![image](https://github.com/akerekon/reflections-research/assets/89589162/9f80315b-5a35-4341-b282-ee611bee7f9f)

This work is based heavily on LLaVA, a visual GPT engine that is great for identifying image content -- but not so much graph content. By generating data for charts using GPT-4, generating corresponding figures based on this data, and developing a dataset of proper responses on questions asked about this data, the authors were able to fine-tune LLaVA to receive far better performance:

![image](https://github.com/akerekon/reflections-research/assets/89589162/41325db3-6230-4385-bed6-7b761b5d6993)

Matplotlib and OCR were combined to both generate figures as well as read textual data from existing figures, achieving description, chart-to-chart, text-to-chart, and chart-editing functionality. This functionality performs not only better than LLaVA itself, but also frameworks specifically designed for chart data extraction:

![image](https://github.com/akerekon/reflections-research/assets/89589162/5fb8962d-99e7-44b6-84e9-78c2aec26e89)

By combining these features with a chatbot, we hope to further expand on this work with our project. We'll focus especially on prompting in a similar manner as these authors:
![image](https://github.com/akerekon/reflections-research/assets/89589162/02bc0564-eceb-4fac-a592-b2a3e14fd388)


