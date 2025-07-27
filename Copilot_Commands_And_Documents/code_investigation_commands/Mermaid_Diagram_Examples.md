# Mermaid Diagram Examples
<!-- Mermaid documentation: https://mermaid.js.org/intro/ -->

## Application Level Diagram

```mermaid
graph TD;
    A[Application] --> B[Library];
    A --> C[Service];
    B --> D[Component];
    C --> D;
```

## Library Level Diagram

```mermaid
graph TD;
    A[Library] --> B[Module];
    A --> C[Helper];
    B --> D[Function];
    C --> D;
```

## Class Level Diagram

```mermaid
classDiagram
    Class01 <|-- AveryLongClass : Cool
    class Class01 {
      >>int<< id
      >>String<< name
      +methodA()
      +methodB()
    }
    class AveryLongClass {
      >>String<< description
      +methodC()
    }
```

## Function Level Diagram

```mermaid
graph TD;
    A[FunctionA] --> B[FunctionB];
    A --> C[FunctionC];
    B --> D[FunctionD];
    C --> D;
```

---

For more complex diagrams and additional examples, please refer to the [Mermaid Live Editor](https://mermaid-js.github.io/mermaid-live-editor/) where you can experiment with Mermaid syntax and see live previews of your diagrams.

Also, check the [Mermaid Documentation](https://mermaid-js.github.io/mermaid/#/) for a comprehensive guide on using Mermaid, including all available diagram types, syntax details, and configuration options.