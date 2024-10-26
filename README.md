# Rust.ia
Building with rust
Rust is a systems programming language focused on safety and performance. It provides memory safety without a garbage collector, making it a popular choice for concurrent and high-performance applications. Below is an overview of Rust features, some example code, and information about licensing.

### Key Features of Rust

1. **Memory Safety**: Rust's ownership system ensures that memory is managed safely without the need for a garbage collector.
2. **Concurrency**: Rust makes it easier to write concurrent code that is free of data races.
3. **Performance**: Rust is designed for high performance, comparable to C and C++.
4. **Zero-Cost Abstractions**: You can use high-level features without sacrificing performance.
5. **Strong Type System**: Rust's type system helps catch errors at compile time.

### Example Code

Here’s a simple example demonstrating Rust’s syntax and features:

```rust
fn main() {
    let name = String::from("Rust");
    println!("Hello, {}!", name);

    // Example of ownership
    let x = 5;
    let y = x; // x is copied, y is a new variable

    println!("x: {}, y: {}", x, y);

    // Example of a vector
    let mut numbers = vec![1, 2, 3];
    numbers.push(4);
    
    for number in &numbers {
        println!("{}", number);
    }

    // Example of a function with ownership
    let my_string = String::from("Hello, Rust!");
    print_string(my_string); // Ownership moved to the function

    // Uncommenting the following line will cause a compile-time error
    // println!("{}", my_string); // Error: my_string has been moved

}

fn print_string(s: String) {
    println!("{}", s);
}
```

### Licensing

Rust is licensed under the **MIT License** and the **Apache License 2.0**, which makes it permissive for both personal and commercial use. You can freely use, modify, and distribute Rust, as long as you comply with the terms of these licenses.

### Conclusion

Rust is a powerful language that emphasizes safety and performance, making it suitable for a wide range of applications, from systems programming to web development. Its ownership model and concurrency features set it apart from many other languages. 

For more information, you can visit the official Rust website: [rust-lang.org](https://www.rust-lang.org).
