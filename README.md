<p align="center">
  <img src="assets/luffy.png" alt="Luffy Logo" width="200" />
</p>

# Luffy Programming Language

Inspired by the adventurous spirit of Monkey D. Luffy from the anime *One Piece*, the Luffy programming language embodies freedom and exploration. As Luffy once said:

> "I don't want to conquer anything. I just think the guy with the most freedom in the entire ocean is the Pirate King."

Luffy, the language, is designed to give developers the freedom to explore programming concepts and live on their own terms, just like the Pirate King. It is simple, expressive, and encourages creativity.

Luffy is a simple, interpreted programming language designed for learning and experimentation. It supports functions, higher-order functions, closures, integers, and arithmetic operations. The language is implemented in Go and features a lexer, parser, evaluator, and REPL.

## Features

- **Integers and Arithmetic**: Perform basic arithmetic operations such as addition, subtraction, multiplication, and division.
- **Booleans and Comparisons**: Use boolean values (`true`, `false`) and comparison operators (`<`, `>`, `==`, `!=`).
- **Functions**: Define and call functions, including higher-order functions.
- **Closures**: Create and use closures for functional programming.
- **Conditionals**: Use `if` and `else` expressions for control flow.

## Examples

### Arithmetic Operations
```luffy
5 + 5 * 2 - 10 / 2  // Result: 10
(2 + 3) * 4         // Result: 20
```

### Boolean Expressions
```luffy
1 < 2               // Result: true
1 > 2               // Result: false
1 == 1              // Result: true
1 != 2              // Result: true
```

### Functions
```luffy
let add = fn(x, y) { x + y; };
add(5, 10);          // Result: 15

let double = fn(x) { x * 2; };
double(4);           // Result: 8
```

### Higher-Order Functions
```luffy
let apply = fn(f, x) { f(x); };
let increment = fn(x) { x + 1; };
apply(increment, 5); // Result: 6
```

### Closures
```luffy
let newAdder = fn(x) {
  fn(y) { x + y; };
};
let addTwo = newAdder(2);
addTwo(3);           // Result: 5
```

### Conditionals
```luffy
if (10 > 5) { 10 } else { 5 };  // Result: 10
if (false) { 1 } else { 2 };    // Result: 2
```

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/luffy.git
   cd luffy
   ```

2. Build the project:
   ```bash
   go build .
   ```

3. Run the REPL:
   ```bash
   ./luffy
   ```

## Running Tests

To run the unit tests, use:
```bash
go test ./...
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Enjoy exploring the Luffy programming language!
