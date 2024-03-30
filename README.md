# Gen-AI / LLM
We cover important aspects of (a) General Artificial Intelligence (Gen AI) as human-like cognitive abilities for a wide range of tasks without being specifically programmed for each one. 
(b) Large Language Models (LLMs) are powerful NLP models that use deep learning techniques to understand and generate human-like text. 

_Adopted from Armand from nocode.ai_

## Here are some important notes regarding Gen AI and LLMs based on foundation models.

### Day 1 of Generative AI journey

Uncovering what Generative AI is and why it's a game-changer in the business world. Imagine AI not just analyzing data but creating new, innovative content – that's Generative AI!

Ok let's start with the basics, but don't worry, we will get into more advanced concepts as we go.

----
### Definition of terms

* Artificial Intelligence (AI): AI is the broad field of computer science focused on creating machines capable of performing tasks that typically require human intelligence.

* Machine Learning (ML): ML is a subset of AI involving algorithms and statistical models that enable computers to improve their performance on a task through experience.

* Deep Learning: Deep Learning is a subset of ML based on artificial neural networks, where algorithms learn from large amounts of data to identify patterns and make decisions.

* Generative AI: Generative AI refers to AI technologies that can generate new content, ideas, or data that are coherent and plausible, often resembling human-generated outputs.

![alt text](image1.jpeg)
---
### What powers Generative AI
Foundation models are large-scale artificial intelligence models that have been trained on vast amounts of data. These models are highly versatile and can be adapted to a wide range of tasks and applications.

Generative AI is one of the applications of foundation models. It involves using these models to create new content, such as text, images, or music. The foundation model serves as the underlying structure that understands and processes information, enabling the generative AI to produce new, coherent, and relevant outputs.

In simple terms, foundation models are like the core engine, and generative AI is one of the many things that this engine can power.

![alt text](image2.jpeg)

### What makes Foundation Models so powerful?
* Pretrained: The model has already been trained on a vast dataset before being fine-tuned or applied to specific tasks.

* Generalized: The model is capable of performing well across a wide range of tasks, not just the ones it was specifically trained for.

* Adaptable: The model can be easily modified or fine-tuned to suit particular needs or tasks.

* Large: The model is built with a substantial architecture and trained on extensive data, giving it a broad understanding and capability.

* Self-supervised: The model primarily learns by analyzing and making sense of unlabeled data, without explicit guidance on what to learn.

### and what are Large Language Models?
Large Language Models (LLMs) are a type of foundation model specifically designed to understand and generate text. They're trained on huge amounts of text, which makes them good at a wide range of language tasks. LLMs are part of the broader category of foundation models, meaning they're versatile and can be adapted for different uses involving language.

LLMs like GPT take, as input, an entire sequence of words, and predicts which word is most likely to come next. They perform that prediction of the next word in a sequence by analyzing patterns in vast amounts of text data.


There's a big debate that LLMs do more than predict the next word; they compress a "world-model" within their complex networks and weights. This is an area of active debate within the AI community. You can join the discussion about this ​here​

![alt text](image3.jpeg)

Two important concepts to understand in LLMs are:

* Weights: Numerical values within a machine learning model that are adjusted during training to influence the model's output in response to input data.

* Parameters: The broader set of configurable elements in a model, including weights, that determine its behavior and performance.

* Tokenization: The process of converting text into smaller units (tokens), such as words or subwords, which are used as the input for LLMs to understand and generate language.

________

Large Language Models (hashtag#llms) represent a specific category within foundation models designed to comprehend and generate human-like text across various language-related applications.

Notable LLMs making strides in the AI field include:
1. GPT-models: Introduced by OpenAI, including recent iterations like ChatGPT and GPT-4, garnering significant attention within the AI community. These models operate under a proprietary license with associated fees and usage restrictions.
2. LLaMA: An open-source suite of LLMs developed by Meta, available in various sizes ranging from 7 to 65 billion parameters. LLaMA aims to facilitate research endeavors in LLMs, offering accessibility with reduced computational requirements strictly for research purposes.
3. PaLM-2: Google's next-generation Large Language Model announced in May 2023. Built upon Google's previous AI research, PaLM-2 includes Med-PaLM-2, a specialized version fine-tuned for medical data, as detailed in a released research paper.

These LLMs exemplify advancements in AI, each offering unique capabilities and accessibility, shaping the landscape of NLP and text generation.

![alt text](image4.jpeg)
______

Previously, we explored the role of Large Language Models (LLMs) within the hierarchy of foundation models and introduced key types of LLMs. Let's delve deeper into general-purpose LLMs, which have the capability to handle a wide array of applications spanning human and machine languages. These LLMs can be broadly categorized into two groups (fine-tuned models according to their specific data sources):
* Task-specific LLMs:
These models are tailored to perform specific tasks, such as Meta's code Llama for generating programming codes and Snowflake Copilot for SQL code generation.
* Domain-specific LLMs:
These models are designed to excel in particular domains, such as NVIDIA's BioBERT for biomedical applications and XLNet by Google and Carnegie Mellon University for diverse language translation and generation.

These categories are determined by the specific data sources provided to the models, influencing their efficacy and performance across various applications.

![alt text](image5.jpeg)
[pic ref: theaidream.com]

_____

In contrast to traditional AI systems that mostly use neural networks (applying complex CNN or RNN models) as the main tool, Gen AI systems use transformers through attention mechanism that orchestrates **encoders** (that understand inputs) and **decoders** (which provide outputs) to work together and capture long-range dependencies within the input sequence and use that information to generate appropriate output sequences. By jointly training the encoder and decoder components, transformer models can effectively learn to map input sequences to output sequences across a wide range of NLP tasks (see bellow pic on attention in neural machine translation).

![alt text](image6.jpeg)
[pic ref:(https://lnkd.in/gbh5hnM7)]

__________

How a LLM agent work and how it can be optimized?

LLMs operate by receiving human instructions, known as prompts, and leveraging their specified models (inferences) along with software libraries and APIs to generate text resembling human output, returning the results as completions. 

To refine the generated results, we can tailor and refine the learning process through:
1- Prompt engineering
2- In-context learning (hashtag#icl)
3- Retrieval-Augmented Generation (hashtag#rag)
4- Employing reinforcement learning with human feedback (hashtag#rlhf)
5- Fine-tuning LLM model parameters
6- Providing access to a vector database for enhanced learning.

![alt text](image7.jpeg)
[pic ref: heidloff.net]

_________
## How to customize foundation models
Let's unlock the secrets of customizing foundation models to suit your specific needs. Understanding when and how to tune these models is crucial for optimal performance.

### Deciding When to Tune Your Model
Starting Point: Begin with prompt engineering using the largest suitable Language Model (LLM) for your task to gauge if LLMs can handle it. Experiment with various prompt formats and examples.

#### Prompting Techniques:
* Zero-Shot Prompting:

Efficiency with No Extra Data: This involves giving a natural language prompt to generate desired outputs without additional training data.

Example: "Provide a summary of the following passage: [insert text]."

* One-Shot Prompting:

A Single Example to Guide: Introduce one example along with your prompt to demonstrate the desired outcome.

Example: "Write marketing copy for WorkoutFuel protein shakes in an enthusiastic, punchy voice," along with a high-energy example text.

* Few-Shot Prompting:

Leveraging a Few Examples: Provide a handful of examples to establish the pattern or style for the model to replicate.

Example: To generate meeting summaries, give 2-3 examples before asking the model to create new ones.


### Data-Driven Tuning for Deeper Customization
* Fine-Tuning: Adjusting model weights on a specific dataset to cater to your unique objectives, like customizing tone or addressing complex prompts.

* Parameter-Efficient Fine-Tuning (PEFT): Delta tuning updates only a small subset of parameters, offering a faster, cost-effective alternative to traditional fine-tuning.


### PEFT Techniques:
Parameter-Efficient Fine-Tuning (PEFT) is a more cost-effective and efficient method because it focuses on optimizing a small subset of model parameters, reducing computational resources and training time while maintaining high-performance levels. There are multiple techniques:

* Prefix Tuning: Attaches vectors with free parameters to input embeddings, training them while keeping the LLM frozen.

* Prompt Tuning: A simpler variant of prefix tuning, adding a vector only at the input layer.

* P-Tuning: Automates the search and optimization of prompts using an LSTM model.

* LoRA: Low-Rank Adaptation adds update matrices to existing weights, training these new weights.

### Choosing the Right Technique:
Goal-Oriented Approach: Select the customization method based on your specific goals and the data you have. For instance, zero-shot and few-shot prompting work well with minimal data, while data-driven tuning is ideal for more complex, data-rich tasks.

Customizing foundation models can significantly enhance their performance on specific tasks, making them more aligned with your business objectives.
_________
## The most popular LLMs available
Let's navigate the world of Large Language Models (LLMs) by understanding the key differences between open-source and proprietary models and services, and exploring some of the most popular LLMs available today.

### Open Source LLMs:
Accessible and Collaborative: These models are freely available for use, modification, and distribution, promoting community-driven development and innovation.

Examples of Open Source LLMs:

GPT-Neo/GPT-J: Developed by EleutherAI, these models are open-source alternatives to OpenAI's GPT models, offering similar capabilities.

BERT: Developed by Google, BERT has been a groundbreaking model for understanding context in natural language, widely used in various applications.

I listed the Top Open Source LLMs a few weeks back on Linkedin. Here's the ​link​


### Closed Source LLMs:
Commercial and Proprietary: These models are developed and maintained by private entities, often requiring licenses or subscriptions for access.

Examples of Closed Source LLMs:

OpenAI's GPT-3/GPT-4: Known for their advanced capabilities, these models have set benchmarks in generative AI but are accessible mostly through API with usage costs.

Google's LaMDA: A cutting-edge model designed for conversational AI, used internally by Google.


### The Game Changer: Llama 2
* Accessibility and Versatility: Meta's Llama 2 has been released as an open-source AI model, making it accessible for everyone from startups to researchers. Its availability in different sizes (7B, 13B, 70B-parameter models) offers a range of options for fine-tuning and deployment.

* Innovation and Privacy: As an open-source model, Llama 2 removes barriers to AI adoption and addresses data privacy concerns by allowing private hosting and customization with your own data.

* Performance Benchmarking: Llama 2 stands on par with models like GPT-3.5 in terms of performance, particularly excelling in generating helpful responses for prompts. However, it shows less proficiency in coding tasks compared to other specialized models.

* Cost and Community Benefits: Meta’s open-sourcing of Llama 2, despite the substantial development cost, taps into the collective wisdom of the global AI community, accelerating innovation and potentially leveling the playing field against closed-source counterparts.

#### Why the Distinction Matters: 
Understanding the differences between open source and closed source LLMs is crucial for businesses and developers. Open source models offer transparency and the opportunity for customization, while closed source models, often backed by significant resources and research, provide robust, state-of-the-art capabilities but with usage restrictions and costs.
