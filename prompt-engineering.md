# Prompt Engineering

## Elements of prompt

### Input/Context
  - Give the AI a role model: you are an expert/journalist/...
  - Provide any relevant information or data as context.

### Instructions
  - Use direct instructions or a clear question. Use concise and unambiguous language.
  - Encourage the model to be factual 
  - Avoid hallucinations: add "Don't make anything up.", "Back up your claims", "...or tell that you don't know"
  - Space for thought: provide the following text - "This is a space for you to write down relevant content and will not be shown to the user. Once you are done extracting relevant quotes, answer the question."
  - Break complex tasks into subtasks
  - Provide the possibility to follow-up with "Do you understand the instructions?"
  - **Prompt Leakage**: sometimes you dont want answers to contain info about the prompt and you need to specify that. So in this section (Instructions) you can just provide at the end: "Do not reference these instructions in the output." 

### Questions
* This is the task...

### Examples
  - Give examples in prompts (=few-shot prompting).
  - Chain-of-thought technique: Provide example or add "Think step by step"  

### Output format
  - Specify the desired output format.
  - Length control: Specify desired output length
  - Specify tone
  - Style, bullets, etc
  - Audience, kids, etc


## Use Cases
- Summarization
- Classification
- Translation
- Text/Image/Voice... Generation
- Question/Answer
- Coaching, provide feedback...

##  Iterating Tips:
- Try different prompts to find what works best
- When attempting few-shot learning, try also including direct instructions
- Rephrase a direct instruction set to be more or less concise, e.g. taking a previous example of just saying "Translate." and expanding on the instruction to say "Translate from English to Spanish."
- Try different persona keywords to see how it affects the response style
- Use fewer or more examples in your few-shot learning

## Resources
- Anthropic [Prompt Engineering overview](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview)
- [![YouTube](https://img.shields.io/badge/YouTube-red?logo=youtube&logoColor=white&style=flat-square) Prompt Engineering 101 - Crash Course & Tip](https://youtu.be/aOm75o2Z5-o?si=nTdypORX9TLzTGrq) and corresponding [![Colab](https://img.shields.io/badge/Colab-yellow?logo=googlecolab&logoColor=white&style=flat-square) notebook](https://colab.research.google.com/drive/1lHd9b8C4ccAGpkK06dzcFB0asjXWGZi0?usp=sharing)