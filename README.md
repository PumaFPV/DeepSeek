# DeepSeek README

This is just a small test extension for running DeepSeekR1 locally. Based from the tutorial of FireShip.

## Features

Ctrl + Shift + P and search for Start DeepSeek. You can then enter your prompt.

## Requirements

npm, ollama and a deepseek model

On windows:
```winget install OpenJS.NodeJS```

```npm install Ollama```

```ollama run deepseek-r1:8b```

## Known issues

For now, anytime you press the Ask button it starts a new conversation and won't remember what was asked previously.

## Release Notes

### 0.0.1

This is just a test to have fun.

## Roadmap

### 0.0.2

Add consersation history with a "Continue button", keep the "Ask" one to start a new conversation.

### 0.0.3

Add a "Save conversation" button to export it in markdown.


## Exemple output
### Prompt
How to do a for loop in cpp

### Answer


To write a for loop in C++, follow these steps:

1. **Start with the `for` keyword.**
2. **Declare variables and initialize them if necessary.** Variables can be declared within the loop, but it's often better to declare them outside if they are needed beyond the loop's scope.
3. **Specify the loop condition using a boolean expression.** The loop will continue as long as this condition is true.
4. **Include an increment or decrement operator (optional).** This allows the loop variable to change with each iteration, controlling the loop's termination.

Here's an example:

```c++
for (int i = 1; i <= 5; i++) {
// Perform some operation on `i`
}
```

- **`for`**: Starts the loop.
- **`int i = 1;`**: Declares an integer `i` initialized to 1.
- **`i <= 5`**: The condition that checks if `i` is less than or equal to 5.
- **`i++`**: Increments `i` after each iteration.

### Example Output:
```plaintext
1
2
3
4
5
```

### Step-by-Step Explanation:

1. **Initialization:** The loop starts by initializing `i` to 1.
2. **Condition Check:** Before the first iteration, the condition `i <= 5` is checked. Since `i` is 1, the loop body executes.
3. **Body Execution:** Inside the loop, operations using `i` are performed.
4. **Increment:** After each iteration, `i` is incremented by 1.
5. **Termination:** When `i` becomes 6 (after incrementing from 5), the condition fails, and the loop exits.

### Usage Scenarios:
- **Counting:** Loop through numbers sequentially.
- **Iteration:** Repeat operations a specified number of times.
- **Control Structures:** Use with other constructs like if statements or switch cases for complex logic.

### Tips:
- **Avoid Multiple Initializations in For Loops:** Declare variables outside the loop to maintain clarity and avoid scope issues.
- **Use `do { } while ();` for guaranteed execution at least once.
- **Ensure Proper Increment/Decrement Steps:** Negative steps allow descending through values, but a zero step leads to infinite loops.

By following these guidelines, you can effectively utilize C++ for loops in your programming tasks.
