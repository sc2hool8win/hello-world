# hello-world
Learning how to use GitHub
1. The guide [here](https://guides.github.com/activities/hello-world/) is for reference.  
1. GitHub's icons : [GitHub Octicons.](https://primer.style/octicons/)

## RUST 
1. hello_world
```C
$rustc main.rs  
$./main  
Hello, world!  
```  
2. hello_cargo
```c
$ cargo new hello_cargo --bin
$ cd hello_cargo 

$ cargo check

$ cargo build
$ ./target/debug/hello_cargo
Hello, world!

$ cargo run
    Finished dev [unoptimized + debuginfo] target(s) in 0.00s
     Running `target/debug/hello_cargo`
Hello, world!

$ cargo build --release
   Compiling hello_cargo v0.1.0 
    Finished release [optimized] target(s) in 0.23s
$ ./target/release/hello_cargo 
Hello, world!  
```  
## C language
1. hello_gnuc
```c
$ cat Makefile
CC := gcc
CFLAGS := -g -Wall -Wextra
hello: 

$ make
$ ./hello
hello, world!
```  
## C++ language
1. hello_cpp
```cpp
$ cat Makefile  
CXX := g++
CXXFLAGS := -g -Wall
hello:

$ make
$ ./hello
Hello world.  
```  
## Python
1. hello_python
```python
$ cat hello.py
#!/usr/bin/env python3.6

def main():
    print("Hello, world!")

if __name__ == '__main__':
    main()

$ ./hello.py
Hello, world!
```  
