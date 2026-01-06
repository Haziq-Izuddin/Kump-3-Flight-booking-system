``` mermaid
flowchart TD
    Start([Start]) --> Input1[/Input Username & Password/]
    Input1 --> Process1[Check Database Records]
    Process1 --> Decision{Credentials Valid?}

    Decision -- Yes --> Output1[/Display "Login Successful"/]
    Output1 --> End([Access Dashboard])

    Decision -- No --> Output2[/Display "Error: Invalid Login"/]
    Output2 --> Decision2{Register New Account?}

    Decision2 -- No --> Input1
    Decision2 -- Yes --> Input3[/Input New User Details/]
    Input3 --> Process2[Save New User to Database]
    Process2 --> Output3[/Display "Registration Complete"/]
    Output3 --> Input1
```
