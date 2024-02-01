# Lunarbat 🦇
Yet another attempt of making a programming language.
 Lunarbat is my Hobby Programming language, making just for learning and fun.

This is just the name of the project, because I didn't choose a good name yet.
 It is called Lunarbat because the bat 🦇 is my favorite animal and the name **BAT**
 was alredy in use

It started as [`Batlang`](https://github.com/vaaako/batlang) but I decide to remake everything
 from scratch, because I was no satisfied with how it was going

# Current State
**Lunarbat** is in very early stage and isn't usable yet

# Goal
### May have changes
This are some of my goals for this language

- Simple
- Fast
- Statically Typed
- Object-oriented

## Desired syntax
```rust
func can_drink(x: int): string {
	if x > 18 {
		return "can drink in Brazil";
	}

	return "can't drink in Brazil";
}


// The object declaration and usage will have changes, this is just an example
const person: Object = {
	info = {
		name: string = "John",
		age: int = 17
	}

	alive: bool = true
};

print(info.name + " has " + info.age + " and he " can_drink(info.age));
```

###  Stuff I coudn't think on a example
```rust
// Declaration and Assigne
let x: int;
x = 123;

// Constants
const PI: float = 3.14;

// Implicity Type
let z = x * y;
```


# Compiling and Running
## Requirements
You need `clang` and `Cmake` *(optional)*
```sh
sudo apt install clang cmake
```

## gcc/clang
```sh
clang++ -std=c++20 -g -O0 -Wall -Qunused-arguments -Werror -Wextra -Wno-sign-compare -Wno-unused-parameter -Wno-unused-variable -Wshadow src/*.cpp src/**/*.cpp -o lunarbat
```


## CMake
Setup the `CMake` environment
```sh
mkdir build
cmake -S . -B build
```

Now you can run
```sh
cmake --build build
```


## SHELL FILE
Alternativally you can use the shell file `run.sh` to automatically compile and run

To run with `make`
```sh
bash run.sh
```

Or run with `CMake`
```sh
bash run.sh -c
```

You can also open `gdb` right after running
```sh
bash run.sh -d
```

And also use [`Valgrind`](https://valgrind.org/)
```sh
bash run.sh -v
```


# Credits
Made by me<br>
Inspired by [Daniel Holden](https://github.com/orangeduck), [Matthew Oros](https://github.com/orosmatthew), [Mika](https://github.com/mikumikudice), [David Callanan](https://github.com/davidcallanan) and [Tyler Laceby](https://github.com/tlaceby) 

## Libraries used
- [`editline`](https://github.com/troglobit/editline)

---
>I'm still learning about `Interpreters` and `C++`, so please let me know if
 I made any mistakes or if you have any suggestions

>If you want to see my notes, see `TODO.md`