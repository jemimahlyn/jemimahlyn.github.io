```mermaid
flowchart TD
    Start([Start])
    Init[Initialize variables and generate a random number]
    Prompt[Prompt user to guess the number]
    Input[User enters a guess]
    Check{Is the guess correct?}
    TooHigh["Too High"]
    TooLow["Too low"]
    Correct["Correct!"]
    End([End])

    Start --> Init --> Prompt --> Input --> Check
    Check -- Too High --> TooHigh --> Prompt
    Check -- Too Low --> TooLow --> Prompt
    Check -- Correct --> Correct --> End
```

## Description 
This flowchart shows the logic of a random number guessing game. The program generates a number, takes input from the user, and gives feedback until the user guesses correctly. 
Based on the guess:
- If it is too high or too low, the user is prompted again.
- If the guess is correct, the program presents a success message and ends. 
