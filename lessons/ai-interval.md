## AI INTERVAL 3.1: ADVANCED PROMPTING & REASONING

### The coffee cart barista training problem.
Advanced prompting is about being specific, structured, and strategic with how you ask AI models to do things for you.
### three key concepts
- Chain-of-thought prompting: How "Think step to step" improves reasoning. Asking an AI model to think step by step before giving as answer.
- structured output with markdown: Forcing consistent, parseable responses. Forcing an AI model to respond in a specific format.
- Two-pass prompting strategy: separating generation from formatting. Using two prompts, one to generate the reasoning, and the other to format the output.
The above concepts are very important when working with AI models. Chain of thought compares the model to think through a process, and give you the process as well rather than just jumping to the final answer, thereby encouraging it to break down a problem into smaller pieces first. For the structured output, it is one of the most useful techniques in prompting. Instead of giving a vague prompt, for a model to do something for you, you specifically outline what and what and in what format you want that model to do that which you want it to do for you. for example, instead of asking a model:
- Explain HTTP
you force a structure:
Explain HTTP using this format: 
- Definition
- How it Works
- Advantages
- Disadvantages
- Example
And finally, the two-pass prompting strategy is employed in the following manner:
instead of asking the model to do everything at once, you split the work into stages:
- one-pass prompting: Generate only the content
- two-pass prompting: Now format it.
This is exactly how it works, you tell the model to think and generate a content for you, and then you give it a format and tell it to format the content it has generated for you into a beautifully formatted output for your consumption.
To properly understand this topic, there are some concepts you need to understand and one of which is:
- markdown. This is a lightweight markup language for formatting text. Used to structure AI responses.
- semantic firewall: This is a security layer that validates user input before it reaches the AI model.