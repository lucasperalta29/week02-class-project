# Week 02 Class Project: Ohm's Law Calculator

## Purpose
A C++ terminal program that calculates electrical current using Ohm's Law (I = V / R).

## Input Format
Two numbers separated by a space: the voltage in volts, then the resistance in ohms.
```
12 4
```
If the input is not numeric, or the resistance is zero or negative, the program prints `Invalid input`.

## Build and Run
Compile:
```
g++ -std=c++17 -Wall -Wextra -pedantic src/main.cpp -o build/app
```
Run the program:
```
./build/app
```
Run all acceptance tests:
```
bash test.sh
```

## Example Output
| Input | Output |
|-------|--------|
| `12 4` | `Current: 3 A` |
| `12 0` | `Invalid input` |

## Limitations
- Only reads one voltage and resistance per run.
- Does not check for extra input after the two numbers.
- Output uses default number formatting, so long decimals are not rounded.

## Debugging Reflection
My first `git push` failed because GitHub does not accept account passwords for Git. I fixed it by creating a personal access token and using it as the password. I also learned that pushing a feature branch to an empty repository does not create a `main` branch, so I created `main` with a README and rebased my feature branch onto it before opening the pull request.
