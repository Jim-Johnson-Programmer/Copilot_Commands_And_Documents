# GitHub Copilot Quick Reference

## Commands
| Command / Prompt                | Description                                                      |
|---------------------------------|------------------------------------------------------------------|
| /help             | Quick reference and basics of using GitHub Copilot.                        |
| /clear            | Clear the current conversation.                                             |
| /delete           | Delete a conversation.                                                      |
| /new              | Start a new conversation or project.                                       |
| /rename           | Rename a conversation.                                                      |
| /explain          | Explain how the code in your active editor works.                          |
| /fix              | Propose a fix for problems in the selected code.                           |
| /fixTestFailure   | Find and fix a failing test.                                                |
| /tests            | Generate unit tests for the selected code.                                 |
| /doc              | Add documentation comment for this symbol.                                 |
| /optimize         | Analyze and improve running time of the selected code.                     |
| /generate         | Generate new code based on a prompt.                                       |
| /simplify         | Simplify selected code.                                                     |
| /feedback         | Provide feedback to GitHub Copilot.                                        |
| /runCommand       | Execute VS Code commands (use with @vscode).                               |
| /test <desc>      | Generate tests for the selected code or file                                |
| /refactor <desc>  | Refactor code as described                                                  |
| /run <command>    | Run a terminal command                                                      |
| /comment          | Add or improve code comments                                                |
| /review           | Review code for issues or improvements                                      |
| /explain error    | Explain the error message or stack trace                                    |
| /summarize        | Summarize the code or file                                                  |

## Variables
> **Note:** Variables start with `#` when used in prompts or scripts. For example: `#workspaceFolder`, `#filePath`.

| Variable Name         | Description                                      |
|----------------------|--------------------------------------------------|
| #workspaceFolder     | The root folder of the current workspace                          |
| #filePath            | The path to the current file                                      |
| #selectedText        | The currently selected text in the editor                         |
| #currentLine         | The line where the cursor is located                              |
| #languageId          | The programming language of the current file                      |
| #repoContext         | Information about the current repository                          |
| #environment_info    | Information about the OS and shell                                |
| #userRequest         | The latest user request or prompt                                 |
| #block               | Includes the current block of code in the prompt.                 |
| #class               | Includes the current class in the prompt.                         |
| #comment             | Includes the current comment in the prompt.                       |
| #file                | Includes the current file's content in the prompt.                |
| #function            | Includes the current function or method in the prompt.            |
| #line                | Includes the current line of code in the prompt.                  |
| #path                | Includes the file path in the prompt.                             |
| #project             | Includes the project context in the prompt.                       |
| #selection           | Includes the currently selected text in the prompt.               |
| #sym                 | Includes the current symbol in the prompt.                        |
| #solution            | References the current solution (used in IDEs like Visual Studio).|

## Participants
| Participant          | Description                                      |
|----------------------|--------------------------------------------------|
| @User                | The person interacting with Copilot                                |
| @GitHub Copilot      | The AI assistant generating code and suggestions                   |
| @VS Code Editor      | The code editor interface                                          |
| @Terminal            | The integrated terminal for running commands                        |
| @Extensions          | Additional tools or plugins in the environment                     |
| @azure               | Has context about Azure services and how to use, deploy, and manage them.  |
| @github              | Enables GitHub-specific Copilot skills.                             |
| @terminal            | Has context about the terminal shell and its contents.              |
| @vscode              | Has context about Visual Studio Code commands and features.         |
| @workspace           | Has context about the code in your workspace/project.               |
| @project             | Considers all files in your project (used in JetBrains IDEs).       |
