# Simple-AI-Agent

This repo based on `Visual Computing Systems Stanford CS348K` course, found at [there](https://gfxcourses.stanford.edu/cs348k/spring24content/media/aiagents1/11_simagents_1_5VsnTc5.pdf).


|![general-llm-agent-arch](https://github.com/user-attachments/assets/80b923f1-df20-4ce9-8e02-d8b44954f5dc)|
|:-----------------------------------:|
|*General LLM Agent Architecture.*|

Normally, a complete LLM agent system will include all components such as: Planning to break down large tasks into small tasks, then deciding which tools to use to solve the tasks or using more memory to help the agent store the history of previous interactions with users.

### LLM

The brain of a LLM Agent is a LLM model which can perform language understanding and natural response ability. 

Input prompt to this LLM is very important to define which plannings, tools or actions that the agent should use and expected answers' format. You also can add a `persona` to this step to fit the agent in particular role and context that help to reduce irrelevant responses. 

### Planning

This step to divide complex tasks to more simple tasks to get the better solutions. 

Planning usually including: `Planning without feedback` and `Planning with feedback`.

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



