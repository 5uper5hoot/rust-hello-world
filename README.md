# Hello, World!

This is the ['Hello, World!'][1] example from [The Rust Programming Languague][2] book.

- Rust files end with the `.rs` extension.
- Convention says to separate words in file names with an underscore (e.g., `hello_world.rs` rather than `helloworld.rs`).

### Functions

```rs
fn main() {

}
```

- The [`fn`][3] keyword:

    > Functions are the primary way code is executed within Rust. 
    > 
    > Function blocks, usually just called functions, can be defined in a variety of different places and be assigned many different attributes and modifiers.

- `main`: The name of the function. `main` is a special name, signifying the first code that will run in an executable rust program.
- `()`: If the fuction had parameters they would go in here.
- `{}`: Function bodies are wrapped in curly braces.

### Expressions

```rs
    println!("Hello, World!");
```

- Indent with 4 spaces, not a tab.
- The `!` signifies this expression calls a [Rust macro][4], not a normal function.
- `"Hello, World!"` is passed as an _argument_ to the [`println!`][5] macro.
- Line ends with `;` signifying that the expression is over and the next can begin.

### Compiling

Rust programs have to be compiled before they can run.

```
> rustc .\main.rs
```

- [`rustc`][6]: The Rust compiler, by Rust, for Rust. Takes source code, and creates binary code.
- `.\main.rs`: Location of the source file.

On Windows, the compiler will produce two files, `main.exe` - the executable, and `main.pdb` - debugging info.

### Executing

Run the executable that was output in the compilation step:

```
> .\main.exe
```

[1]: https://doc.rust-lang.org/book/ch01-02-hello-world.html
[2]: https://doc.rust-lang.org/book/title-page.html
[3]: https://doc.rust-lang.org/std/keyword.fn.html
[4]: https://doc.rust-lang.org/book/ch19-06-macros.html
[5]: https://doc.rust-lang.org/std/macro.println.html
[6]: https://doc.rust-lang.org/rustc/index.html