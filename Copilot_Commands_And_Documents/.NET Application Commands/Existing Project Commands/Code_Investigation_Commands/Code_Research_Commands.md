# Code Research Commands Cheat Sheet

| Command                                      | Description                                      |
|----------------------------------------------|--------------------------------------------------|
| <span class="copy-btn">/copySolution &lt;destination_folder&gt;</span>           | Copy full solution to another companion folder    |
| <span class="copy-btn">/removeGitTracking &lt;solution_folder&gt;</span>         | Remove git tracking from a copied solution folder |


## Generating Command Line Explanation of Existing Code
| Command                        | Description                        |
|--------------------------------|------------------------------------|
| <span class="copy-btn">/explainSolution</span>               | Explain the full solution          |
| <span class="copy-btn">/explainProject</span>                | Explain the project                |
| <span class="copy-btn">/explainClass &lt;class_name&gt;</span>     | Explain the specified class        |
| <span class="copy-btn">/explainFunction &lt;function_name&gt;</span> | Explain the specified function   |
| <span class="copy-btn">/explainVariable &lt;variable_name&gt;</span> | Explain the specified variable   |

## Generating Command Line Comments for Existing Code (for code not accessible to git)
| Command                          | Description                                      |
|----------------------------------|--------------------------------------------------|
| <span class="copy-btn">/commentSolution</span>                 | Add a personal comment to the full solution      |
| <span class="copy-btn">/commentProject</span>                  | Add a personal comment to the project            |
| <span class="copy-btn">/commentClass &lt;class_name&gt;</span>       | Add a personal comment to the specified class    |
| <span class="copy-btn">/commentFunction &lt;function_name&gt;</span> | Add a personal comment to the specified function |
| <span class="copy-btn">/commentVariable &lt;variable_name&gt;</span> | Add a personal comment to the specified variable |

---

## Diagnostic Research for Issues

Use these commands to help diagnose and research issues in your codebase:

| Command                                 | Description                                      |
|------------------------------------------|--------------------------------------------------|
| <span class="copy-btn">/findBugsSolution</span>                       | Identify potential bugs in the full solution     |
| <span class="copy-btn">/findBugsProject</span>                        | Identify potential bugs in the project           |
| <span class="copy-btn">/findBugsClass &lt;class_name&gt;</span>              | Identify potential bugs in the specified class   |
| <span class="copy-btn">/findBugsFunction &lt;function_name&gt;</span>        | Identify potential bugs in the specified function|
| <span class="copy-btn">/findBugsVariable &lt;variable_name&gt;</span>        | Identify potential bugs in the specified variable|
| <span class="copy-btn">/suggestFixesSolution</span>                    | Suggest fixes for issues in the full solution    |
| <span class="copy-btn">/suggestFixesProject</span>                     | Suggest fixes for issues in the project          |
| <span class="copy-btn">/suggestFixesClass &lt;class_name&gt;</span>          | Suggest fixes for the specified class            |
| <span class="copy-btn">/suggestFixesFunction &lt;function_name&gt;</span>    | Suggest fixes for the specified function         |
| <span class="copy-btn">/suggestFixesVariable &lt;variable_name&gt;</span>    | Suggest fixes for the specified variable         |

---

## Custom Research Commands

Use these commands to perform custom research or analysis tasks on your codebase:

| Command                                   | Description                                         |
|--------------------------------------------|-----------------------------------------------------|
| <span class="copy-btn">/searchCode &lt;search_term&gt;</span>                  | Search for a term or pattern in the codebase        |
| <span class="copy-btn">/listDependencies</span>                          | List all dependencies in the solution or project    |
| <span class="copy-btn">/findUsage &lt;symbol_name&gt;</span>                   | Find all usages of a class, function, or variable   |
| <span class="copy-btn">/summarizeFile &lt;file_path&gt;</span>                 | Summarize the contents of a specific file           |
| <span class="copy-btn">/summarizeChanges &lt;commit_or_branch&gt;</span>       | Summarize code changes in a commit or branch        |
| <span class="copy-btn">/compareFiles &lt;file1&gt; &lt;file2&gt;</span>              | Compare two files and highlight differences         |
| <span class="copy-btn">/generateTestCases &lt;function_or_class&gt;</span>     | Generate test cases for a function or class         |

---

## Mermaid Diagram Examples

See [Mermaid_Diagram_Examples.md](./Mermaid_Diagram_Examples.md) for prompts, responses, and sample markup for generating Mermaid diagrams at the application, library, class, and function levels.

---

<!--
To enable copy-on-click for these commands in Markdown preview, you can use a browser extension or VS Code extension that supports copying content from HTML spans with a specific class. For web docs, add a small JS snippet to handle click-to-copy for `.copy-btn`.
-->



