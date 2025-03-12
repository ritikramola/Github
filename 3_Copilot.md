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

# Codespaces

## The Codespace lifecycle
GitHub Codespaces is configurable, allowing you to create a customized development environment for your project. By configuring a custom development environment for your project, you can have a repeatable Codespace configuration for all users of your project.

A Codespace's lifecycle begins when you create a Codespace and ends when you delete it. You can disconnect and reconnect to an active Codespace without affecting its running processes. You can stop and restart a Codespace without losing the changes that you make to your project.

## Create a Codespace
You can create a Codespace on GitHub.com, in Visual Studio Code, or by GitHub CLI. There are four ways to create a Codespace:

    From a GitHub template or any template repository on GitHub.com to start a new project.
    From a branch in your repository, for new feature work.
    From an open pull request, to explore work-in-progress.
    From a commit in a repository's history to investigate a bug at a specific point in time.
You can temporarily use a Codespace in order to test code or you can return to the same Codespace to work on long-running feature work.

You can create more than one Codespace per repository or even per branch. However, there are limits to the number of Codespaces you can create and run at the same time. When you reach the maximum number of Codespaces and try to create another, a message is displayed. The message tells you that an existing Codespace needs to be removed/deleted before a new Codespace can be created.

You can create a new Codespace each time you develop in GitHub Codespaces or keep a long-running Codespace for a feature. If starting a new project, create a Codespace from a template and publish it to a repository on GitHub later.

When creating a new Codespace each time you work on a project, you should regularly push your changes to ensure that any new commits are on GitHub. When using a long-running Codespace for a new project, pull from the repository's default branch each time you start working in Codespace to enable your environment to get the latest commits. The workflow is similar to working with a project on a local machine.

Repository administrators can enable GitHub Codespaces prebuilds for a repository to speed up Codespace creation.

### Codespace creation process
Diagram of a GitHub codespace and how it connects from your code editor and into a docker container.

When you create a GitHub Codespace, four processes occur:

    A virtual machine and storage are assigned to your Codespace.
    A container is created.
    A connection to the Codespace is made.
    A post-creation setup is made.

### Save changes in a Codespace
When you connect to a Codespace through the web, AutoSave is automatically enabled to save changes after a specific amount of time passes. When you connect to a Codespace through Visual Studio Code running on your desktop, you must enable AutoSave.

Your work saves to a virtual machine in the cloud. You can close and stop a Codespace and return to the saved work at a later time. If you have unsaved changes, you receive a prompt to save them before exiting. However, if your Codespace is deleted, then your work is lost. To save your work, you must commit your changes and push them to your remote repository or publish your work to a new one if you created your Codespace from a template.

### Open an existing Codespace
You can reopen any of your active or stopped Codespaces on GitHub.com, in a JetBrains IDE, in Visual Studio Code, or by using GitHub CLI.

To resume an existing Codespace, you can go to the repository where the Codespace exists, select the , key and then select Resume this codespace. Or, you can open https://github.com/codespaces in the browser, select the repository, and then select the existing Codespace.

### Timeouts for a Codespace
If a Codespace is inactive, or if you exit your Codespace without explicitly stopping, the application times out after a period of inactivity and stops running. The default timeout is after 30 minutes of inactivity. When a Codespace times out, your data is kept from the last time your changes were saved.

## Close or stop a Codespace
If you exit the Codespace without running the stop command or leave the Codespace running without interaction, the Codespace and its running processes continue during the inactivity timeout period. The default inactivity timeout period is 30 minutes. You can define your personal timeout setting for the Codespaces you create, but an organization's timeout policy can overrule the setting.

Only running Codespaces incur CPU charges. A stopped Codespace incurs only storage costs.

You can stop and restart a Codespace to apply changes. For example, if you change the machine type used for your Codespace, you need to stop and restart it for the change to take effect. When you close or stop your Codespace, all uncommitted changes are preserved until you connect to the Codespace again.

You can also stop Codespace and choose to restart or delete it if you encounter an error or something unexpected.

## Rebuild a Codespace
You can rebuild your Codespace to implement changes to your dev container configuration. For most uses, you can create a new Codespace as an alternative to rebuilding a Codespace. When you rebuild your Codespace, images from the cache speed-up the rebuild process. You can also perform a full rebuild to clear the cache and rebuild the container with fresh images.

When you rebuild the container in a Codespace, changes you made outside the /workspaces directory are cleared. Changes you made inside the /workspaces directory, including the clone of the repository or template you created the Codespace from, are preserved over a rebuild.

## Delete a Codespace
You can create a Codespace for a particular task. After you push your changes to a remote branch, then you can safely delete that Codespace.

If you try to delete a Codespace with unpushed git commits, the editor notifies you that you have changes that aren't yet pushed to a remote branch. You can push any desired changes and then delete your Codespace. You can also continue to delete your Codespace and any uncommitted changes or export the code to a new branch without creating a new Codespace.

Stopped Codespaces that remain inactive for a specified amount of time are deleted automatically. Inactive Codespaces delete after 30 days, but you can customize your Codespace retention intervals.

## Personalize your Codespace
GitHub Codespaces is a dedicated environment for you. You can configure your repositories with a dev container to define their default GitHub Codespaces environment and personalize your development experience across all of your Codespaces with dotfiles and Settings Sync.

### What you can customize
There are many ways you can customize your Codespace. Let's review each one.

1.Settings Sync: You can synchronize your Visual Studio Code (VS Code) settings between the desktop application and the VS Code web client.

2.Dotfiles: You can use a dotfiles repository to specify scripts, shell preferences, and other configurations.

3.Rename a Codespace: When you create a Codespace, an autogenerated display name is assigned to it. If you have multiple Codespaces, the display name helps you to differentiate between Codespaces. You can change the display name for your Codespace.

4.Change your shell: You can change your shell in a Codespace to keep the setup you're used to. When you're working in a Codespace, you can open a new terminal window with a shell of your choice, change your default shell for new terminal windows, or install a new shell. You can also use dotfiles to configure your shell.

5.Change the machine type: You can change the type of machine that's running your Codespace, so that you're using resources appropriate for the work you're doing.
Set the default editor: You can set your default editor for Codespaces in your personal settings page. Set your editor preference so that when you create a Codespace or open an existing Codespace, it opens to your default editor.
    Visual Studio Code (desktop application)
    Visual Studio Code (web client application)
    JetBrains Gateway - for opening Codespaces in a JetBrains IDE
    JupyterLab - the web interface for Project Jupyter
6.Set the default region: You can set your default region in the GitHub Codespaces profile settings page to personalize where your data is held.

7.Set the timeout: A Codespace will stop running after a period of inactivity. By default this period is 30 minutes, but you can specify a longer or shorter default timeout period in your personal settings on GitHub. The updated setting applies to any new Codespaces you create, or to existing Codespaces the next time you start them.

8.Configure automatic deletion: Inactive Codespaces are automatically deleted. You can choose how long your stopped Codespaces are retained, up to a maximum of 30 days.

Additional information and step-by-step instructions regarding customization are located in the Summary unit at the end of this module.

### Add to your Codespace with extensions or plugins
You can add plugins and extensions within a Codespace to personalize your experience in JetBrains and VS Code.

#### VS Code extensions
If you work on your Codespaces in the VS Code desktop application or the web client, you can add any extensions you need from the Visual Studio Code Marketplace. Refer to Supporting Remote Development and GitHub Codespaces in the VS Code documentation for information on how extensions run in GitHub Codespaces.

If you already use VS Code, you can use Settings Sync to automatically sync extensions, settings, themes, and keyboard shortcuts between your local instance and any Codespaces you create.