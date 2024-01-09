# Objective
1. Learn about Large Language Models
2. Poor with no access to the closed source models such as GPT4 but would like to keep the ability to use them in the future
3. Understand and use "Agents"
4. Create a program that can research and write blogs

Based on my research, here are some of the components I will be using 

1. Ollama
2. CrewAI



# Ollama: Large Language Models, Demystified
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
You are convinced. You have installed WSL2 and have access to bash. Let's talk a little out the programming language and interface we will be using to accomplish our task.

The preferred programming language for Data Scientists is Python. And the interface I will choose today is Visual Studio Code. The short answer to why I am choosing this editor is the ability to write both complex Python packages and simple notebooks for testing code. You can learn more about Visual Studio Code [here](https://code.visualstudio.com/docs). Implement the simple example provided [here](https://code.visualstudio.com/docs/python/python-tutorial) to ensure that your machine and environment is fully set up. 
























Here is the full blog post:

Title: Exploring the Latest Features of Torizon OS and TorizonCore - A Comprehensive Guide for Tech Enthusiasts!

Hey there, fellow tech enthusiasts! Today, we're diving into the latest features of Torizon OS and TorizonCore. Why, you ask? Well, because our mission is to make complex tech concepts accessible and exciting for all of you!

Imagine this: You're cooking up a storm in your smart kitchen, and suddenly, something goes wrong with your connected appliances. No need to panic! With Torizon OS and TorizonCore, you can now enjoy the peace of mind that comes with Remote Access Client (RAC) integration. This feature will allow you to connect to your appliances from anywhere, anytime, making your smart kitchen even smarter!

But wait, there's more! The team behind Torizon Core has been working hard to enhance the security of their platform by adding support for secure boot in their latest features. You know what that means? Your data is safer than ever before! It's like having a bodyguard for your precious information.

And if you think that was impressive, wait until you hear about their new device drivers. Torizon OS and TorizonCore now support Microchip KSZ8795/KSZ88X3 switch chips, making them compatible with more devices than ever before! It's like upgrading your favorite gadget to work with a wider range of accessories.

Oh, and let's not forget about TorizonCore 5.7.2, the latest maintenance release focused on improving stability and reliability for use in embedded Linux software development. This update follows the recent release of TorizonCore 6.1.0, which brings new features to Toradex's System on Modules. It's like getting a brand-new toolbox filled with helpful gadgets!

But hold your horses, because there's an even bigger upgrade on the horizon - the upcoming Torizon OS 6 update with a bootloader upgrade. Just imagine what that could mean for the future of IoT devices and applications! The possibilities are endless.\n\nSo there you have it, folks! The latest features of Torizon OS and TorizonCore in a nutshell. We hope we've made this tech journey as exciting as possible, proving once again that complex doesn't always mean complicated. Keep an eye on these innovative platforms, as the future looks brighter than ever!

Windows Subsystem for Linux (WSL)
WSL2 is the latest version of the Windows Subsystem for Linux, which allows Windows users to access the Linux kernel directly. It has become increasingly popular due to its ease of use and interoperability between Windows and Linux. Some of the most popular facts about WSL2 include:

WSL2 uses a virtualized Linux kernel with less overhead compared to traditional virtual machines, making it more efficient.
The system call compatibility between WSL2 and Linux is full, allowing for seamless integration between the two operating systems.
WSL2 makes it easy to share files between Windows and Linux environments without requiring extra work.
Users can choose from various Linux distributions available on the Microsoft Store or install WSL2 using PowerShell.
The Windows Terminal is a recommended tool for working with terminals in Windows, as it provides a modern, fast, and efficient experience.
It's easier to use WSL2 compared to traditional virtual machines or dual-boot setups, as no modifications are needed for Linux applications, utilities, and Bash command-line tools.
Developers can leverage the full power of Linux on Windows 10 and Windows 11, making it an invaluable tool for their work.
As for the trending aspects of WSL2, some topics that have gained recent attention include:

Performance comparisons between WSL2 and native Ubuntu installations
The integration of WSL2 with the Windows Terminal for a more streamlined experience
The use of WSL2 for containerization and Docker development on Windows
The compatibility of various Linux distributions within the WSL2 environment
Best practices for setting up multiple profiles in WSL2 using the Windows Terminal
Welcome to the exciting world of WSL2! As a tech-savvy user, you may already be familiar with the concept of a virtual machine or dual-boot setup to run Linux on your Windows machine. But what if I told you there's a better way? That's where WSL2 comes in.

WSL2 stands for Windows Subsystem for Linux 2, and it is Microsoft's latest innovation that allows users to access the Linux kernel directly from their Windows machines. This means you can now run Linux applications, utilities, and Bash command-line tools without needing a separate Linux installation or dual-boot setup. And the best part? It's easier and more efficient than ever before!

With WSL2, users can enjoy full system call compatibility between Windows and Linux, making it simple to share files between the two environments without any extra work. This virtualized Linux kernel is also more efficient than traditional virtual machines, using less overhead to provide a faster and smoother experience.
