# Cross Compiler on Windows

1. setup cross-compiler
```dos
rustup target add x86_64-unknown-linux-gnu
```
2. set Crgo.toml 
```dos
[package]
name = "hello_world"
version = "0.1.0"
authors = ["Your Name <you@example.com>"]
edition = "2018"

[profile.release]
lto = true
opt-level = "z"
strip = true

[target.x86_64-unknown-linux-gnu]
linker = "x86_64-linux-gnu-gcc"
```
3. Compilation Execution
```dos
cargo build --release --target x86_64-unknown-linux-gnu 
> error: linker `cc` not found
```

4. add: Microsoft C++ Build Tools OR Visual Studio Community  
   1. http: [learn.microsoft.com](https://learn.microsoft.com/ja-jp/windows/dev-environment/rust/setup)

5. MYSYS2 Install
    1. [mysys2.org](https://www.msys2.org/)
    1. start menu `MSYS2 MSYS`  for windows
    
```dos
pacman -Syu
    $ pacman -S --needed base-devel mingw-w64-x86_64-toolchain
```
>Error



```bash
pacman -Syu  # update
pacman -S base-devel  
pacman -S msys2-devel  
```


