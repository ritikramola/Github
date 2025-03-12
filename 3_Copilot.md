# GitHub Copilot, your AI pair programmer

It's no secret that AI is disrupting the technology landscape. AI is profoundly changing the way the world works and how each organization and team operates. These advancements in AI serve as a catalyst and can dramatically improve the productivity of developers around the world as they use and apply it well.

The addition of AI features to the developer tools that you use and love helps you collaborate, develop, test, and ship your products faster and more efficiently than ever before. GitHub Copilot is a service that provides you with an AI pair programmer that works with all of the popular programming languages.

In recent research, GitHub and Microsoft found that developers experience a significant productivity boost when they use GitHub Copilot to work on real-world projects and tasks. In fact, in the three years since its launch, developers have experienced the following benefits while using GitHub Copilot:

    46% of new code now written by AI
    55% faster overall developer productivity
    74% of developers feeling more focused on satisfying work

Microsoft developed GitHub Copilot in collaboration with OpenAI. GitHub Copilot is powered by the OpenAI Codex system. OpenAI Codex has broad knowledge of how people use code and is more capable than GPT-3 in code generation. OpenAI Codex is more capable, in part, because it was trained on a dataset that included a larger concentration of public source code.

GitHub Copilot is available as an extension for VS Code, Visual Studio, Vim/Neovim, and the JetBrains suite of IDEs.

## GitHub Copilot features
GitHub Copilot started a new age of software development as an AI pair programmer that keeps developers in the flow by autocompleting comments and code. But AI-powered autocompletion was just the starting point.

Here are some features of GitHub Copilot that truly make it a developer tool of the future. With these features, GitHub Copilot is more than just an editor. It's becoming a readily accessible AI assistant throughout the entire development life cycle.

### Copilot for chat
GitHub Copilot brings a ChatGPT-like chat interface to the editor. The chat interface focuses on developer scenarios and natively integrates with VS Code and Visual Studio. It's deeply embedded in the IDE, and it recognizes what code a developer has typed and what error messages appear. A developer can get in-depth analysis and explanations of what code blocks are intended to do, generate unit tests, and even get proposed fixes to bugs.

### Copilot for pull requests
OpenAI's GPT-4 model adds support in GitHub Copilot for AI-powered tags in pull-request descriptions through a GitHub app that organization admins and individual repository owners can install. GitHub Copilot automatically fills out these tags based on the changed code. Developers can then review or modify the suggested descriptions.

### Copilot for the CLI
Next to the editor and pull requests, the terminal is the place where developers spend the most time. However, even the most proficient developers need to scroll through many pages to remember the precise syntax of many commands. The GitHub Copilot command-line interface (CLI) can compose commands and loops, and it can and throw obscure find flags to satisfy your query.

## Subscription plans
The service is available through GitHub personal accounts with GitHub Copilot Free and GitHub Copilot Pro, through organization accounts with GitHub Copilot Business, or through enterprise accounts with GitHub Copilot Enterprise.

### GitHub Copilot Business
GitHub Copilot Business allows you to control who can use GitHub Copilot in your company. After you give access to an organization, its admins can give access to individuals and teams.

With GitHub Copilot Business, GitHub Copilot is open to every developer, team, organization, and enterprise.

With the following features, GitHub Copilot Business is focused on making organizations more productive, secure, and fulfilled:

    Code completions
    Chat in IDE and mobile
    Filter for security vulnerabilities
    Code referencing
    Filter for public code
    IP indemnity
    Enterprise-grade security, safety, and privacy
    GitHub Copilot Enterprise
    GitHub Copilot Enterprise is available for organizations through GitHub Enterprise Cloud. This subscription plan enables your teams of developers to:

Quickly get up to speed on your codebase.
Search through and build documentation.
Get suggestions based on internal and private code.
Quickly review pull requests.
GitHub Copilot Enterprise includes everything in GitHub Copilot Business, plus a layer of personalization for organizations. It provides integration into GitHub as a chat interface, so developers can converse about their codebase. It also provides action buttons throughout the platform.

GitHub Copilot Enterprise can index an organization's codebase for a deeper understanding and for suggestions that are more tailored. It offers access to GitHub Copilot customization to fine-tune private models for code completion.

## Interact with Copilot
This unit explores ways that you can maximize your interaction with GitHub Copilot in your development environment. By understanding the service's features and capabilities, you'll learn how to use it effectively.

The following sections describe the various ways to trigger and use GitHub Copilot, along with examples and shortcuts to help you get the most out of it.

### Inline suggestions
Inline suggestions are the most immediate form of assistance in Copilot. As you type, Copilot analyzes your code and context to offer real-time code completions. This feature predicts what you might want to write next and displays suggestions in a subtle, unobtrusive way.

The suggestions that Copilot offers appear as grayed-out text ahead of your cursor.

To accept a suggestion, select the Tab key or the > (right arrow) key.
To reject a suggestion, keep typing or select the Esc key.

### Command palette
The command palette provides quick access to the various functions in Copilot, so you can perform complex tasks with only a few keystrokes.

Open the command palette in Visual Studio Code by selecting Ctrl+Shift+P (Windows or Linux) or Cmd+Shift+P (Mac).
Enter Copilot to see available commands.
Select actions like Explain This or Generate Unit Tests to get assistance.

### Copilot chat
Copilot chat is an interactive feature that enables you to communicate with Copilot by using natural language. You can ask questions or request code snippets, and Copilot provides responses based on your input.

Open the Copilot chat panel in your IDE.
Enter questions or requests in natural language, and then evaluate the Copilot response.

### Inline chat
Inline chat enables context-specific conversations with Copilot directly within your code editor. You can use this feature to request code modifications or explanations without switching contexts.

Place your cursor where you want assistance.
Use the keyboard shortcut Ctrl+I (Windows or Linux) or Cmd+I (Mac) to open inline chat.
Ask questions or request changes specific to that code location.
Inline chat helps you focus on a particular section of your code and get targeted advice.

### Comments to code
Copilot uses natural language processing to convert comments into code. You can describe the functionality that you want in a comment. When you select the Enter key, Copilot generates code based on your description.

### Multiple suggestions
For complex code snippets, Copilot can offer multiple alternatives.

When Copilot offers a suggestion, look for the light bulb icon.
Select the icon or use Alt+] (Windows/Linux) or Option+] (Mac) to cycle through alternatives.
Multiple suggestions help you explore different coding approaches and select the most appropriate one.

### Explanations
Understanding existing code is crucial, especially in large projects. You can use the Explain This feature to get explanations for code snippets.

    Select a block of code.
    Right-click the code block, and then select Copilot: Explain This on the shortcut menu.
    Read the explanation that Copilot provides for the selected code.
This feature is useful for learning purposes and when you're reviewing code that someone else wrote.

### Automated test generation
Unit tests are essential for ensuring code quality and reliability. Copilot can save you time and effort by generating unit tests for your functions or classes.

    Select a function or class.
    Use the command palette to select Copilot: Generate Unit Tests.
    Review the test cases that Copilot suggests for your code.

