mermaid ```
flowchart TD
    X(Game Starts)
    X--> A[[Computer creates a number]]
    A --> B[User makes a guess]
    B --> C[/User makes an input/]
    C--> D[Input is too high]
    C --> E[Input is too low] 
    D --> B 
    E --> B
    C --> F[Input is the right number]
    F --> G(Game Ends)
```