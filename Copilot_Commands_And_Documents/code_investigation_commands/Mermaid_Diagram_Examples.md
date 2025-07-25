# Mermaid Diagram Examples
<!-- Mermaid documentation: https://mermaid.js.org/intro/ -->

Mermaid supports a wide variety of diagram/chart types for visualizing code, workflows, and data. For full details, see the [Mermaid documentation](https://mermaid.js.org/intro/).

**Common Mermaid Diagram Types:**
- **Flowchart** – Visualize processes, logic, and workflows.
- **Sequence Diagram** – Show interactions between components or objects over time.
- **Class Diagram** – Represent classes, methods, and relationships (UML style).
- **State Diagram** – Model state machines and transitions.
- **Entity Relationship Diagram** – Describe database tables and their relationships.
- **User Journey** – Map user journeys and experiences.
- **Gantt** – Visualize project timelines and schedules.
- **Pie Chart** – Display data proportions.
- **Quadrant Chart** – Show data in four quadrants.
- **Requirement Diagram** – Visualize requirements and dependencies.
- **GitGraph (Git) Diagram** – Illustrate Git branching and commits.
- **C4 Diagram** – Model software architecture at different abstraction levels.
- **Mindmaps** – Organize ideas and concepts hierarchically.
- **Timeline** – Show events in chronological order.
- **ZenUML** – Alternative sequence diagram syntax.
- **Sankey** – Visualize flow and distribution of resources.
- **XY Chart** – Plot data points on X/Y axes.
- **Block Diagram** – Represent system components and their connections.
- **Packet Diagram** – Visualize network packet flows.
- **Kanban** – Model Kanban boards for workflow management.
- **Architecture Diagram** – Show system or infrastructure architecture.
- **Radar Chart** – Compare multivariate data.
- **Treemap** – Visualize hierarchical data as nested rectangles.

## Rendering the Code as Diagrams

**Approach 1: GitHub in Browser**
- Push your Markdown file(s) to GitHub.
- View the file in your browser; GitHub will render Mermaid diagrams automatically.

**Approach 2: VS Code Plugin**
- **VS Code Mermaid Diagram Preview:**  
  To view Mermaid diagrams rendered as images locally in VS Code:
  1. Install the [Markdown Preview Mermaid Support](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid) extension, the [Mermaid Preview](https://marketplace.visualstudio.com/items?itemName=vstirbu.vscode-mermaid-preview) extension, and the [Auto-Open Markdown Preview](https://marketplace.visualstudio.com/items?itemName=hnw.vscode-auto-open-markdown-preview) extension.
  2. Open your Markdown file containing Mermaid code blocks.
  3. With "Auto-Open Markdown Preview" installed, the preview tab will open automatically when you open a Markdown file.
  4. The Mermaid code will be rendered in the viewer tab.
  5. For `.mmd` files, use the "Mermaid Preview" extension and open the preview pane.

---

## Copilot Application Commands to Generate Diagrams

Use the following commands to generate each type of diagram for your application.  
Click the copy button to quickly copy any command.

```plaintext
/generateMermaidDiagram application flowchart
```
```plaintext
/generateMermaidDiagram application sequence
```
```plaintext
/generateMermaidDiagram application class
```
```plaintext
/generateMermaidDiagram application state
```
```plaintext
/generateMermaidDiagram application erd
```
```plaintext
/generateMermaidDiagram application userjourney
```
```plaintext
/generateMermaidDiagram application gantt
```
```plaintext
/generateMermaidDiagram application pie
```
```plaintext
/generateMermaidDiagram application quadrant
```
```plaintext
/generateMermaidDiagram application requirement
```
```plaintext
/generateMermaidDiagram application gitgraph
```
```plaintext
/generateMermaidDiagram application c4
```
```plaintext
/generateMermaidDiagram application mindmap
```
```plaintext
/generateMermaidDiagram application timeline
```
```plaintext
/generateMermaidDiagram application zenuML
```
```plaintext
/generateMermaidDiagram application sankey
```
```plaintext
/generateMermaidDiagram application xy
```
```plaintext
/generateMermaidDiagram application block
```
```plaintext
/generateMermaidDiagram application packet
```
```plaintext
/generateMermaidDiagram application kanban
```
```plaintext
/generateMermaidDiagram application architecture
```
```plaintext
/generateMermaidDiagram application radar
```
```plaintext
/generateMermaidDiagram application treemap
```

**Tip:**  
Replace `application` with `library <library_name>`, `class <class_name>`, or `function <function_name>` as needed to generate diagrams for other codebase levels.

## Copilot Library Commands to Generate Diagrams

Use the following commands to generate each type of diagram for your library.  
Click the copy button to quickly copy any command.

```plaintext
/generateMermaidDiagram library <library_name> flowchart
```
```plaintext
/generateMermaidDiagram library <library_name> sequence
```
```plaintext
/generateMermaidDiagram library <library_name> class
```
```plaintext
/generateMermaidDiagram library <library_name> state
```
```plaintext
/generateMermaidDiagram library <library_name> erd
```
```plaintext
/generateMermaidDiagram library <library_name> userjourney
```
```plaintext
/generateMermaidDiagram library <library_name> gantt
```
```plaintext
/generateMermaidDiagram library <library_name> pie
```
```plaintext
/generateMermaidDiagram library <library_name> quadrant
```
```plaintext
/generateMermaidDiagram library <library_name> requirement
```
```plaintext
/generateMermaidDiagram library <library_name> gitgraph
```
```plaintext
/generateMermaidDiagram library <library_name> c4
```
```plaintext
/generateMermaidDiagram library <library_name> mindmap
```
```plaintext
/generateMermaidDiagram library <library_name> timeline
```
```plaintext
/generateMermaidDiagram library <library_name> zenuML
```
```plaintext
/generateMermaidDiagram library <library_name> sankey
```
```plaintext
/generateMermaidDiagram library <library_name> xy
```
```plaintext
/generateMermaidDiagram library <library_name> block
```
```plaintext
/generateMermaidDiagram library <library_name> packet
```
```plaintext
/generateMermaidDiagram library <library_name> kanban
```
```plaintext
/generateMermaidDiagram library <library_name> architecture
```
```plaintext
/generateMermaidDiagram library <library_name> radar
```
```plaintext
/generateMermaidDiagram library <library_name> treemap
```

**Tip:**  
Replace `<library_name>` with the name of your library to generate diagrams for that specific library.

## Copilot Class Commands to Generate Diagrams

Use the following commands to generate each type of diagram for your class.  
Click the copy button to quickly copy any command.

```plaintext
/generateMermaidDiagram class <class_name> flowchart
```
```plaintext
/generateMermaidDiagram class <class_name> sequence
```
```plaintext
/generateMermaidDiagram class <class_name> class
```
```plaintext
/generateMermaidDiagram class <class_name> state
```
```plaintext
/generateMermaidDiagram class <class_name> erd
```
```plaintext
/generateMermaidDiagram class <class_name> userjourney
```
```plaintext
/generateMermaidDiagram class <class_name> gantt
```
```plaintext
/generateMermaidDiagram class <class_name> pie
```
```plaintext
/generateMermaidDiagram class <class_name> quadrant
```
```plaintext
/generateMermaidDiagram class <class_name> requirement
```
```plaintext
/generateMermaidDiagram class <class_name> gitgraph
```
```plaintext
/generateMermaidDiagram class <class_name> c4
```
```plaintext
/generateMermaidDiagram class <class_name> mindmap
```
```plaintext
/generateMermaidDiagram class <class_name> timeline
```
```plaintext
/generateMermaidDiagram class <class_name> zenuML
```
```plaintext
/generateMermaidDiagram class <class_name> sankey
```
```plaintext
/generateMermaidDiagram class <class_name> xy
```
```plaintext
/generateMermaidDiagram class <class_name> block
```
```plaintext
/generateMermaidDiagram class <class_name> packet
```
```plaintext
/generateMermaidDiagram class <class_name> kanban
```
```plaintext
/generateMermaidDiagram class <class_name> architecture
```
```plaintext
/generateMermaidDiagram class <class_name> radar
```
```plaintext
/generateMermaidDiagram class <class_name> treemap
```

**Tip:**  
Replace `<class_name>` with the name of your class to generate diagrams for that specific class.

## Copilot Function Commands to Generate Diagrams

Use the following commands to generate each type of diagram for your function.  
Click the copy button to quickly copy any command.

```plaintext
/generateMermaidDiagram function <function_name> flowchart
```
```plaintext
/generateMermaidDiagram function <function_name> sequence
```
```plaintext
/generateMermaidDiagram function <function_name> class
```
```plaintext
/generateMermaidDiagram function <function_name> state
```
```plaintext
/generateMermaidDiagram function <function_name> erd
```
```plaintext
/generateMermaidDiagram function <function_name> userjourney
```
```plaintext
/generateMermaidDiagram function <function_name> gantt
```
```plaintext
/generateMermaidDiagram function <function_name> pie
```
```plaintext
/generateMermaidDiagram function <function_name> quadrant
```
```plaintext
/generateMermaidDiagram function <function_name> requirement
```
```plaintext
/generateMermaidDiagram function <function_name> gitgraph
```
```plaintext
/generateMermaidDiagram function <function_name> c4
```
```plaintext
/generateMermaidDiagram function <function_name> mindmap
```
```plaintext
/generateMermaidDiagram function <function_name> timeline
```
```plaintext
/generateMermaidDiagram function <function_name> zenuML
```
```plaintext
/generateMermaidDiagram function <function_name> sankey
```
```plaintext
/generateMermaidDiagram function <function_name> xy
```
```plaintext
/generateMermaidDiagram function <function_name> block
```
```plaintext
/generateMermaidDiagram function <function_name> packet
```
```plaintext
/generateMermaidDiagram function <function_name> kanban
```
```plaintext
/generateMermaidDiagram function <function_name> architecture
```
```plaintext
/generateMermaidDiagram function <function_name> radar
```
```plaintext
/generateMermaidDiagram function <function_name> treemap
```

**Tip:**  
Replace `<function_name>` with the name of your function to generate diagrams for that specific function.

