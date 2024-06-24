In this blog-style tutorial, I will be working towards the following objectives.

1. Understand Large Language Models (LLMs).
2. Open-source vs. Closed-source models
3. Focus on open-source models rather than the closed-source ones. Open-source models are free to download and train. Documented models show the number of parameters and the data that the model was trained on, unlike closed source models where we do not understand the number of parameters or the data that the model was trained on.
4. Keep the cost as close as possible to zero. Use infrastructure created to download and test different open-source models locally. No special tools that require subscriptions or limited access and none that I will need to pay for since I am only testing them to understand capabilities. 
5. Understand and use "Agents"
6. Use points 1 through 4 to create a blog researcher and writer. 


## What are Large Language Models?

Large Language Models, or "LLMs", are the latest buzzwords in the world of artificial intelligence (AI) and natural language processing (NLP). These models are AI systems trained on vast amounts of text data, enabling them to generate human-like text and understand complex linguistic patterns. They have significant potential implications for society, ranging from improving customer service chatbots to revolutionizing creative writing, from poetry to code snippets. LLMs are the result of years of research in AI and NLP. 

The first language models, such as Recurrent Neural Networks (RNNs) and Long Short-Term Memory (LSTM), laid the groundwork for today's powerful LLMs. Fast forward to recent years, and we have witnessed a remarkable evolution in language processing capabilities. GPT-4, developed by OpenAI, is one such example of a state-of-the-art LLM with 176 billion parameters. 

They are primarily based on Transformer architectures, introduced by Vaswani et al. in their seminal paper "Attention is All You Need." The Transformer model utilizes self-attention mechanisms to understand the context of words within a sentence, making it an efficient and scalable method for processing long sequences of text.


## Open-source Vs. Closed-source

The world of AI is ever-evolving, and understanding the difference between open-source and closed-source LLMs can be crucial in finding the right balance for your needs. Whether you're a small business trying to streamline operations or an individual looking for personalized recommendations, choosing between open and closed-source LLMs will depend on the specifics of your situation. The important thing is to stay informed and make decisions that align with your goals and values.

**Open-source LLMs**
Advantages  | Disadvantages
------------- | -------------
Control over Training Data | Performance
Cost-Effectiveness | Limited Development Resources
Customizable Applications | 

**Closed-source LLMs**
Advantages  | Disadvantages
------------- | -------------
Potential for Better Performance | Potential Misuse of AI
Support from Large Companies and Additional Development Resources | Can get expensive based on the task


## What will I be using to achieve my objective
Based on my research, here are some of the components I will be using 

1. **Operating system:** Linux on Windows with WSL2
2. **Code editor:** Visual Studio Code
3. **Programming Language:** Python
4. **Libraries and other components:**
    1. CrewAI
    2. Ollama


## CrewAI
What is better than an agent? Multiple agents. [CrewAI](https://github.com/joaomdmoura/crewAI) is a framework for orchestrating role-playing, autonomous AI agents. By fostering collaborative intelligence, CrewAI empowers agents to work together seamlessly, tackling complex tasks. CrewAI works with local models downloaded via Ollama or remote models like OpenAI.


## Ollama: Large Language Models, Demystified
You're trying to build an AI-powered chatbot for your business. You want it to be smart, efficient, and able to handle complex queries. But the popular language models out there have long waiting lists, and registration is a hassle. What do you do? Enter Ollama, the open-source hero who's here to save the day!

Ollama is a platform designed for running, managing, and building local applications with large language models (LLMs). It's like having your very own AI lab right at your fingertips. But what makes Ollama so special? Let's dive in:

1. **Flexibility is Key**: Ollama lets you customize and create your models using the "Modelfile" format, giving you the freedom to tailor your LLM to your specific needs.
2. **Popular Models, Supported**: Whether you're a fan of Llama 2, Code Llama, OPT, or PaLM, Ollama has got you covered with its extensive library.
3. **API Savvy**: Need to serve your models via gRPC or HTTP APIs? Ollama's got you covered there too! It's all about the seamless integration.
4. **Conversational Champions**: Ready to take on conversational agents? Ollama helps you create chatbots and assistants that can carry on intelligent conversations with your users.
5. **Performance Perks**: Ollama optimizes performance, ensuring your large language models run smoothly even on lower-end hardware. It also plays well with cloud services like Fly.io for a faster experience.
6. **Open-Source Advancements**: By using Ollama, you're not only avoiding registration and waitlists but also leveraging the latest advancements in open-source large language models for your applications.

With Ollama, you can ditch the waiting lists and enjoy the benefits of cutting-edge AI technology without any fuss.


## but .. (there is always one)
As of the time of writing this blog, Ollama is not available on Windows. It has been released for MacOS and Linux. This puts some developers at a significant disadvantage as the thought of programming in Linux sends shivers down some spines. Some time ago, the only way to experience Linux was to have it installed in a separate space on your machine. This was cumbersome and the files were not shared without significant effort. Do you remember the times when Microsoft used to hate Linux and did everything in its power to stop integration in the name of "security"? Well, I am glad to inform the few who have not kept up with the advancements that Microsoft now loves Linux. We have now got WSL2 or the second version of "Windows Subsystem for Linux".


## Windows Subsystem for Linux (WSL)
WSL2 is the latest version of the Windows Subsystem for Linux, which allows Windows users to access the Linux kernel directly. It has become increasingly popular due to its ease of use and interoperability between Windows and Linux. Some of the most popular facts about WSL2 include:

  - WSL2 uses a virtualized Linux kernel with less overhead compared to traditional virtual machines, making it more efficient.
  - The system call compatibility between WSL2 and Linux is full, allowing for seamless integration between the two operating systems.
  - WSL2 makes it easy to share files between Windows and Linux environments without requiring extra work.
  - Users can choose from various Linux distributions available on the Microsoft Store or install WSL2 using PowerShell.
  - The Windows Terminal is a recommended tool for working with terminals in Windows, as it provides a modern, fast, and efficient experience.
  - It's easier to use WSL2 compared to traditional virtual machines or dual-boot setups, as no modifications are needed for Linux applications, utilities, and Bash command-line tools.
  - Developers can leverage the full power of Linux on Windows 10 and Windows 11, making it an invaluable tool for their work.

Allowing users to access the Linux kernel directly from their Windows machines, you can now run Linux applications, utilities, and Bash command-line tools without needing a separate Linux installation or dual-boot setup. It's easier and more efficient than ever before. With WSL2, users can enjoy full system call compatibility between Windows and Linux, making it simple to share files between the two environments without any extra work. This virtualized Linux kernel is also more efficient than traditional virtual machines, using less overhead to provide a faster and smoother experience.

Use this [link](https://learn.microsoft.com/en-us/windows/wsl/about) to understand more about WSL2, and this [link](https://learn.microsoft.com/en-us/windows/wsl/install) on how to enable it on your Windows machine. 


## What next? (Part one)
You are convinced. You have installed WSL2 and have access to bash. Let's talk a little about the programming language and interface we will be using to accomplish our task.

The preferred programming language for Data Scientists is Python. And the interface I will choose today is Visual Studio Code. The short answer to why I am choosing this editor is the ability to write both complex Python packages and simple notebooks for testing code. You can learn more about Visual Studio Code [here](https://code.visualstudio.com/docs). Implement the simple example provided [here](https://code.visualstudio.com/docs/python/python-tutorial) to ensure that your machine and environment are fully set up. 


## Let's begin
For ease of explainability, I will be using a notebook. The full code can be found on GitHub

**Step 0:** Prerequisites 

Run the following code snippets once per project build, on the terminal.

```
pip install langchain
```
Installs the LangChain library

```
pip install crewai
```
Installs the CrewAI library

```
pip install duckduckgo-search
```
Install the DuckDuckGo-Search library

```
ollama pull openhermes
``` 
Pulls the model into the local system. "openhermes" is the model and can be replaced with any of the models hosted by Ollama.

**Step 1:** Import the libraries for CrewAI and LangChain

```
from crewai import Agent, Task, Crew
from langchain_community.tools import DuckDuckGoSearchRun
```

**Step 2:** Import Ollama and initialize the llm

```
from langchain.llms import Ollama
ollama_llm = Ollama(model="openhermes")
```

**Step 3:** Import and initialize DuckDuckGo and create a search tool
```
from crewai_tools import tool
@tool("Duck_Duck_Go_Search")
def ddgsearch(question: str) -> str:
    """Clear description for what this tool is useful for, your agent will need this information to use it."""
    # Function logic here
    return DuckDuckGoSearchRun().run(question)
```
This is used to provide the model access to the internet. 

**Step 4:** Introducing a variable called "research_topic". This variable should be changed in your code to try out different topics.
```
research_topic = "Differences between open source large language models and closed source large language models."
```

**Step 5:** Configure the first agent. I am going with the "Researcher".

```
researcher = Agent(
  role='Researcher',
  goal='Search the internet about {research_topic}',
  backstory="""
  You are a researcher. Using the information in the task, you find out some of the most popular facts about the topic along with some of the trending aspects.
  You provide a lot of information thereby allowing a choice in the content selected for the final blog
  """,
  verbose=True,            # want to see the thinking behind
  allow_delegation=False,  # Not allowed to ask any of the other roles
  # tools=[DuckDuckGoSearchRun()],
  tools=[ddsearch],        # Is allowed to use the following tools to conduct research
  llm=ollama_llm           # local model
)
```

**Step 6:** Configure the second agent. I am going to call this the "Technical Content Creator".

```
writer = Agent(
  role='Tech Content Strategist',
  goal='Craft compelling content on a set of information provided by the researcher.',
  backstory="""You are a writer known for your humorous but informative way of explaining. 
  You transform complex concepts into compelling narratives.""",
  verbose=True,            # want to see the thinking behind
  allow_delegation=True,   # can ask the "researcher" for more information
  llm=ollama_llm           # using the local model
)
```

**Step 7:** Define the task that needs to be done by the "Researcher". Call this "Task1"

```
task1 = Task(
  agent=researcher,
  description=research_topic,
  expected_output="A complete analysis of the {research_topic}, presented as a report.",
)
```

**Step 8:** Define the task that needs to be done by the "Technical Content Creator". Call this "Task2"

```
task2 = Task(
  agent=writer,
  description="""Using the insights provided, develop an engaging blog
  post that highlights the most significant facts and differences between open-source LLMs and closed-source LLMs.
  Your post should be informative yet accessible, catering to a tech-savvy audience.
  Make it sound simple, and avoid complex words so it doesn't sound AI generated.""",
  expected_output="""A article containing a minimum of 4 paragraphs. contains no more than 2500 words but no less than 1500 words.
  The final output will not contain any extra fluff like "Paragraph 1:" or any action the writer should do.""",
)
```

**Step 9:** Instantiate the "crew" with a sequential process

```
crew = Crew(
  agents=[researcher, writer],
  tasks=[task1, task2],
  verbose=2, # You can set it to 1 or 2 for different logging levels
)
```

**Step 10:**  Get your crew to start work

```
result = crew.kickoff()
```

Here is an example of an output provided by the Crew

Title: Exploring the Latest Features of Torizon OS and TorizonCore - A Comprehensive Guide for Tech Enthusiasts!

Hey there, fellow tech enthusiasts! Today, we're diving into the latest features of Torizon OS and TorizonCore. Why, you ask? Well, because our mission is to make complex tech concepts accessible and exciting for all of you!

Imagine this: You're cooking up a storm in your smart kitchen, and suddenly, something goes wrong with your connected appliances. No need to panic! With Torizon OS and TorizonCore, you can now enjoy the peace of mind that comes with Remote Access Client (RAC) integration. This feature will allow you to connect to your appliances from anywhere, anytime, making your smart kitchen even smarter!

But wait, there's more! The team behind Torizon Core has been working hard to enhance the security of their platform by adding support for secure boot in their latest features. You know what that means? Your data is safer than ever before! It's like having a bodyguard for your precious information.

And if you think that was impressive, wait until you hear about their new device drivers. Torizon OS and TorizonCore now support Microchip KSZ8795/KSZ88X3 switch chips, making them compatible with more devices than ever before! It's like upgrading your favorite gadget to work with a wider range of accessories.

Oh, and let's not forget about TorizonCore 5.7.2, the latest maintenance release focused on improving stability and reliability for use in embedded Linux software development. This update follows the recent release of TorizonCore 6.1.0, which brings new features to Toradex's System on Modules. It's like getting a brand-new toolbox filled with helpful gadgets!

But hold your horses, because there's an even bigger upgrade on the horizon - the upcoming Torizon OS 6 update with a bootloader upgrade. Just imagine what that could mean for the future of IoT devices and applications! The possibilities are endless.\n\nSo there you have it, folks! The latest features of Torizon OS and TorizonCore in a nutshell. We hope we've made this tech journey as exciting as possible, proving once again that complex doesn't always mean complicated. Keep an eye on these innovative platforms, as the future looks brighter than ever!

## Conclusion
Pretty for a first attempt. And the kicker; large sections of this post were written by this AI implementation! The example was validated by a human and the rating provided was a 5 out of 10. The limitation stated was that the information provided was old. BUT, a good first draft. 

Most implementation frameworks provide models but with no connection to the internet to fetch the latest information. For example, [LMStudio](https://lmstudio.ai/) is an exciting way to test new open-source models locally. The best bit is that the interface shows you the models you can run on your local systems and the ones that will not run due to system limitations like the availability of RAM. With DuckDuckGo-Search, we gave the model access to the internet.

## What's next
Providing context to the model, via documents or a VectorDB. We will soon be testing how pre-trained models perform when asking questions about the documents or DB that we provide. 

