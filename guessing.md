### Guessing a number 1 through 100
```mermaid  
flowchart TD  
A[Start Game] --> B[Initialize Secret Number 1 - 100]
B --> C[Prompt User Input]
C --> D[Check if user input is valid]  
D --> E([No])
E --> C
D --> F([Yes])
F --> G[Check if user input is the secret number]
G --> H([No])
H --> HH[Check if input is higher or lower than secret number]
HH --> H1[Higher than secret number output: Lower]
HH --> H2[Lower than secret number output: Higher]
H1 --> C
H2 --> C
G --> I([Yes])
I --> J[Congratulate user on winning the game]
J --> K[End Game]

```