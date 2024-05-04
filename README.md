# ReAct-Agent

This Python script demonstrates a conversational agent implemented using the ReAct framework and various language processing tools. 

**Summary:**
1. **get_text_length Function:** This function calculates the length of a text input by counting the number of characters. It strips any leading or trailing non-alphanumeric characters before calculating the length.
2. **find_tool_by_name Function:** This function searches for a tool by its name within a list of tools. It iterates through the list of tools and returns the tool object if found. If the tool is not found, it raises a `ValueError`.
3. **Main Script Execution:**
   - **Prompt Template:** Defines a template for the conversation prompts, including placeholders for questions, thoughts, actions, inputs, observations, and final answers.
   - **Agent Initialization:** Initializes the conversational agent with the specified language model (in this case, ChatOpenAI) and sets up callback handlers.
   - **Agent Invocation:** The script enters a loop where the agent interacts with the user to answer questions and perform actions based on the provided input.
   - **Agent Action Execution:** The agent invokes the appropriate tool based on the user's input question. It executes the action defined by the tool, collects observations, and updates intermediate steps.
   - **Agent Finish:** Once the agent completes the conversation or reaches a finishing condition, it prints the final answer or return values.
5. **Callback Handler:** The `AgentCallbackHandler` class is responsible for handling callbacks during the agent's execution. It processes intermediate steps and manages the flow of the conversation.

Overall, the script demonstrates how to build a conversational agent using the ReAct framework, integrating language processing tools, prompts, and output parsing to facilitate natural language interactions. It showcases a simple example of answering questions and performing actions based on user input.
