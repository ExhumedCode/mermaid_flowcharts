flowchart TD
    A([START]) --> B[/Display welcome message and prompt/]
    B --> C[/Get user input/]
    C --> D{Is input 'exit'?}
    D -->|Yes| E([END])
    D -->|No| F{Is input valid?}
    F -->|No| G[/Display error message/]
    G --> B
    F -->|Yes| H[/Display table header/]
    H --> I[Compute and display table<br>number * i for i in 1..10]
    I --> J[/Display blank line/]
    J --> B
