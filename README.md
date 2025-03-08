# libft
Libft is the first project of the 42 Core Program. It aims to get students to create a library of utility functions that can be used in any future C project, and also servers as revision of programming concepts covered in the the 1-month Piscine coding bootcamp, prior to the core program

## 📖 Main concepts covered
- Coverage of the basics of C: E.g. Functions, pointers, memory allocation and freeing etc.
- Newer concepts such as Header files and linking, makefile and compiling into libraries, linkedlists
This project is split into mandatory and a bonus section. The bonus consist of all functions in mandatory, alongside additional utility functions relating to linkedlists

## ⬇️ Clone this repository

```
git clone git@github.com:Sheldon-Chong/libft.git
```

## ⏯️ Compile and run

Compile mandatory
```zsh
make
```

Compile bonus section
```zsh
make bonus
```


## My experience with the Libft
Overall, Libft was fairly straightforward. It was like doing a series of small puzzles, a few of which were more difficult than others.
One of the main challenges I encountered was deciding how much complex functions should rely on other functions within the library. For example, functions like `ft_split` and `ft_atoi` naturally depend on more fundamental functions such as `ft_strlen` and `ft_strdup`. This raised the question of whether to re-define these basic functions statically within the same file containing the more complex functions, to allow their use independently of the library.

My final decision was to keep it simple and have functional interdependance when nescessary. I realised that I would likely require using these functions alongside each other, under the compiled library of libft, so it wasn't nescessary to ensure functions worked independantly outside the library.
