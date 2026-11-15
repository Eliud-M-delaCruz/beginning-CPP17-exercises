# Learning C++17

Working through *Beginning C++17, 5th Edition* (Apress) to learn C++. I already have experience with C# (Unity game development) and some Python, so this repo is about hands-on practice with C++ and programming fundamentals, plus getting more comfortable with Git and GitHub.

## Layout

Each chapter has its own folder (`Ch01`, `Ch02`, ...) containing that chapter's exercises, named like `Ex1_01.cpp`.

## How to Build

The root `CMakeLists.txt` uses `add_subdirectory(...)` to point at one chapter folder at a time. Each chapter folder has its own `CMakeLists.txt` with `add_executable(...)`, which builds the `.exe` for that exercise. To build a different chapter, change the folder name in the root `add_subdirectory(...)` line.

```
cmake -S . -B build
cmake --build build
```

## Setup and What I Learned

I decided to do as much as possible from the terminal, since a GUI isn't always available. I've used the Ubuntu terminal a fair amount in the past, but I'd forgotten some basics, like copying files and folders between directories. I got around that with research and problem solving, which is a programmer's best skill.

The process:

1. **Organized the project.** One folder per chapter. My first problem was that CMake needed to know each folder builds its own exercise. The fix was a root `CMakeLists.txt` pointing at subdirectories, plus one `CMakeLists.txt` per chapter holding the `add_executable` call.
2. **Moved files from the terminal.** My first attempt to copy the CMake file into `Ch01` landed it in the `build` folder, and I mangled its name while fixing that, so I had to rename it and then move it to the right directory. Annoying, but a good exercise.
3. **Initialized Git** and added a `.gitignore` so the `build` folder isn't pushed.
4. **Connected to GitHub.** GitHub's auto-generated initial commit gave me an "unrelated histories" error, which I resolved by pulling with `--allow-unrelated-histories`. That dropped me into Vim, so I looked up how to get out by saving the changes, and the merge went through.
5. **Renamed `master` to `main`** so the local branch matches GitHub.

## Progress

- [x] Chapter 1
- [ ] Chapter 2 (in progress)
- [ ] Chapter 3
- [ ] Chapter 4
- [ ] Chapter 5
- [ ] Chapter 6
- [ ] Chapter 7
- [ ] Chapter 8
- [ ] Chapter 9
- [ ] Chapter 10
- [ ] Chapter 11
- [ ] Chapter 12
- [ ] Chapter 13
- [ ] Chapter 14
- [ ] Chapter 15
- [ ] Chapter 16
- [ ] Chapter 17
- [ ] Chapter 18
