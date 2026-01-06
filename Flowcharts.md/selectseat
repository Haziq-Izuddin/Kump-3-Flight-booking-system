``` mermaid
flowchart LR
    Start([Start]) --> Input1[/User Selects Flight/]
    Input1 --> Process1[Retrieve Seat Map Data]
    Process1 --> Output1[/Display Seat Layout/]

    Output1 --> Input2[/User Clicks Specific Seat/]
    Input2 --> Decision{Is seat available?}

    Decision -- No --> Error[/Error: Seat Taken/]
    Error --> Output1

    Decision -- Yes --> Process2[Lock Seat & Update Status]
    Process2 --> Process3[Save Selection to Booking]

    Process3 --> End([Proceed to Payment])
```
