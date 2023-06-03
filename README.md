# Comet Programming Language

Comet is a modern, high-level programming language designed for simplicity, productivity, and performance. It aims to provide an intuitive and expressive syntax while leveraging the power of existing runtime environments. This README file provides an overview of Comet and guides you on how to get started.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Syntax](#syntax)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Features

Comet offers a range of features that make it a versatile language for various programming tasks:

- **Simplicity**: Comet's syntax is designed to be intuitive and easy to understand, making it accessible to beginners and experts alike.
- **Productivity**: The language promotes clean and concise code, reducing boilerplate and unnecessary complexity.
- **Performance**: Comet leverages the power of underlying runtime environments to deliver high-performance applications.
- **Interoperability**: It seamlessly integrates with existing libraries and frameworks, allowing you to leverage their functionality.
- **Concurrency**: Comet provides built-in support for concurrency, enabling efficient and scalable concurrent programming.
- **Error Handling**: The language incorporates robust error handling mechanisms to handle exceptions and errors gracefully.

## Installation

To start using Comet, you need to follow these installation steps:

1. Visit the official [Comet Website](https://okuretakodimo.github.io/comet/).
2. Download the latest stable release for your operating system.
3. Follow the installation instructions provided for your specific platform.
4. Verify the installation by opening a terminal or command prompt and running the following command:

```shell
comet --version
```

If the installation was successful, you should see the version of Comet installed on your system.

## Getting Started

Once Comet is installed, you can start writing and executing your programs. Follow these steps to get started:

1. Create a new file with the `.comet` extension, for example, `hello.comet`.
2. Open the file in your favorite text editor or integrated development environment (IDE).
3. Write your Comet code in the file.
4. Save the file and navigate to the directory containing it using the terminal or command prompt.
5. To run your Comet program, execute the following command:

```shell
comet hello.comet
```

The above command will compile and execute your `hello.comet` program.

## Syntax

Comet's syntax is designed to be expressive and human-readable. Here's a brief overview of some of the language's syntax features:

### Variables

You can declare variables in Comet using the `let` keyword:

```comet
let x = 42
```

### Functions

Functions in Comet are defined using the `func` keyword:

```comet
class Greet:
  func greet(name):
    traceln("Hello, " + name + "!")
  end

  func main():
    let name = "John"
    greet(name)
  end
end
```

### Control Flow

Comet supports control flow structures like conditionals and loops:

```comet
class ConditionLoop:
  func main():
    let x = 15
    if x > 10:
      traceln("x is greater than 10")
    else:
      traceln("x is less than or equal to 10")
    end

    let i = 0
    while i < 10:
      i = i + 1
    end
  end
end
```

### Error Handling

Comet provides a built-in mechanism for error handling using the `try` and `catch` keywords:

```comet
class Divide:
  func divide(a, b):
    if b == 0:
      throw "Division by zero"
    end
    return a / b
  end

  func main():
    try:
      let result = divide(10, 0)
      traceln(result)
    catch error:
      traceln("An error occurred: " + error)
    end
  end
end
```

For

 more detailed information about Comet's syntax and features, refer to the official documentation.

## Examples

To see Comet in action, here are a few examples showcasing different programming scenarios:

- **Hello, World!**

```comet
class HelloWorld:
  func main():
    traceln("Hello, World!");
  end
end
```

- **Fibonacci Series**

```comet
class Fibonacci:
  func fibonacci(n):
    if n <= 1:
      return n;
    end
    return fibonacci(n - 1) + fibonacci(n - 2);
  end

  func main():
    let num = 10
    traceln("Fibonacci series up to " + num + ":");
    for i in 0..num:
      traceln(fibonacci(i));
    end
  end
end
```

Feel free to explore more examples in the [examples](./examples) directory of this repository.

## Contributing

Contributions to Comet are welcome! If you want to contribute to the language or its documentation, please follow the guidelines outlined in the [CONTRIBUTING](./CONTRIBUTING.md) file.

## License

Comet is open-source software released under the [MIT License](./LICENSE). You are free to use, modify, and distribute Comet according to the terms of this license. Please refer to the [LICENSE](./LICENSE) file for more information.
