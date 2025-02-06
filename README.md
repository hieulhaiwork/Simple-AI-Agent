# Simple-LLM-Agent

Someone calls AI Agent and the other says LLM Agent. At this time, I would say they're the same thing but to classify them clearly, LLM Agent should be understood as LLM-based AI Agent. For example, in the future, imagine that there would be a machine learning model which can replace the LLM's tasks at present so it might be called ML Agent :)

It's easy to understand, right? Then, let's deep dive into the details.

## I. Intro

Inspired by [Visual Computing Systems Stanford CS348K](https://gfxcourses.stanford.edu/cs348k/spring24content/media/aiagents1/11_simagents_1_5VsnTc5.pdf) course and [What are AI Agents?](https://www.youtube.com/watch?v=F8NKVhkZZWI) from IBM Technology channel, I create this repo as a personal study of AI Agent to answer questions: what is it and how to use it?

*Firstly, what is AI Agent?*

Simply, AI Agent is a software that can make decisions to complete particular tasks without given rules or help of human but through its knowledge and interations with the real world.

*Why AI Agent?*

The need of AI Agent is originated from the limitations of base LLM model:
- Knowledge (out of date, lack of fields, bias,...)
- Hard to adapt to particular tasks

## II. Components

|![general-llm-agent-arch](https://github.com/user-attachments/assets/80b923f1-df20-4ce9-8e02-d8b44954f5dc)|
|:-----------------------------------:|
|*General LLM-based Agent Architecture.*|

Normally, a complete LLM agent system will include: 
- `Planning` to break down large tasks into small tasks, this step's also known as reasoning step - the core of a LLM agent.
- `Actions` are all things the agent can interact with the world by tools, such as: searching, calculating,....
- The agent also need to define when to use and how to use `tools` to achieve the best solution.
- `Memory` is where to store its Chain of thought in the past for future planning or history of chat for personal optimizing.

### LLM

The brain of a LLM Agent is a LLM model which can perform language understanding and natural response ability. 

Input prompt to this LLM is very important to define which plannings, tools or actions that the agent should use and expected answers' format. You also can add a `persona` to this step to fit the agent in particular role and context that help to reduce irrelevant responses. 

### Planning

This step to divide complex tasks to more simple tasks to get the better solutions. Planning usually including: `Planning without feedback` and `Planning with feedback`.

#### Planning without feedback
- Chain of thoughts
- Tree of thoughts

#### Planning with feedback
- Reflection

### Memory

#### Short-term memory
This is where agent can store temporital context of conversation to get better responses but will be renewed after finishing the task.

#### Long-term memory
Simply imagine that this like a diary of agent, storing all knowledge of agent from several days, months or even years. Based on these knowledge, agent may handle new tasks that have never seen before but of course, they must be relevant to previous tasks.

### Tools
These tools help agent to do their work, they also have to know in which context, which tools they should use.



