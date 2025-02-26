# Rust Guessing Game

This is a simple Rust program that allows the user to input a guess and prints it back to them.

## Description

The program prompts the user to input a number as a guess and then prints the guess back to them. This example demonstrates basic user input handling in Rust using the `std::io` module.

## Code

```rust
use std::io;

fn main() {
    println!("Guess the number!");

    println!("Please input your guess.");

    let mut guess = String::new();

    io::stdin()
        .read_line(&mut guess)
        .expect("Failed to read line");

    println!("You guessed: {}", guess);
}
```

## How to Run

Ensure you have Rust installed. If not, install it from [rust-lang.org](https://www.rust-lang.org/).

1. Save the Rust code to a file, e.g., `main.rs`.
2. Open a terminal and navigate to the directory containing `main.rs`.
3. Compile and run the program using:
   ```sh
   rustc main.rs
   ./main
   ```

## Expected Output

```
Guess the number!
Please input your guess.
42  # (User inputs a number)
You guessed: 42
```

## License
This project is open-source and free to use.
