*This project has been created as part of the 42 curriculum by [alerradi].*
# libft

A custom C library reimplementing standard libc functions from scratch, built as part of the 42 school curriculum.

## Overview

`libft` is a foundational project that involves recreating a set of standard C library functions along with additional utility functions. The goal is to build a personal, reusable library that can be used throughout future 42 projects.

## Functions

### Character Checks & Conversions
| Function | Description |
|---|---|
| `ft_isalnum` | Check if character is alphanumeric |
| `ft_isalpha` | Check if character is alphabetic |
| `ft_isascii` | Check if character is a valid ASCII character |
| `ft_isdigit` | Check if character is a digit |
| `ft_toupper` | Convert character to uppercase |
| `ft_tolower` | Convert character to lowercase |

### String Functions
| Function | Description |
|---|---|
| `ft_strlen` | Get length of a string |
| `ft_strchr` | Locate first occurrence of character in string |
| `ft_strrchr` | Locate last occurrence of character in string |
| `ft_strdup` | Duplicate a string |
| `ft_strjoin` | Concatenate two strings into a new one |
| `ft_strtrim` | Trim characters from start and end of string |
| `ft_strsplit` / `ft_split` | Split string by delimiter into array |
| `ft_strncmp` | Compare two strings up to n characters |
| `ft_strnstr` | Locate substring in string, within n characters |
| `ft_strlcat` | Concatenate strings with size bound |
| `ft_strlcpy` | Copy string with size bound |
| `ft_strmapi` | Apply function to each character of string |
| `ft_striteri` | Apply function to each character with index |
| `ft_substr` | Extract substring from string |

### Memory Functions
| Function | Description |
|---|---|
| `ft_memset` | Fill memory with a constant byte |
| `ft_memcpy` | Copy memory area |
| `ft_memmove` | Copy memory area, handling overlap |
| `ft_memchr` | Scan memory for a character |
| `ft_memcmp` | Compare two memory areas |
| `ft_bzero` | Zero out a block of memory |
| `ft_calloc` | Allocate and zero-initialize memory |

### Conversion Functions
| Function | Description |
|---|---|
| `ft_atoi` | Convert string to integer |
| `ft_itoa` | Convert integer to string |

### Output Functions
| Function | Description |
|---|---|
| `ft_putchar_fd` | Write a character to a file descriptor |
| `ft_putstr_fd` | Write a string to a file descriptor |
| `ft_putendl_fd` | Write a string followed by newline to a file descriptor |
| `ft_putnbr_fd` | Write an integer to a file descriptor |

### Linked List Functions (Bonus)
| Function | Description |
|---|---|
| `ft_lstnew` | Create a new linked list node |
| `ft_lstadd_front` | Add node to front of list |
| `ft_lstadd_back` | Add node to back of list |
| `ft_lstsize` | Count nodes in list |
| `ft_lstlast` | Get last node of list |
| `ft_lstdelone` | Delete a single node |
| `ft_lstclear` | Delete all nodes in list |
| `ft_lstiter` | Iterate over list and apply function |
| `ft_lstmap` | Map a function over list and return new list |

## Compilation

```bash
make        # Build the library (libft.a)
make bonus  # Build with linked list functions
make clean  # Remove object files
make fclean # Remove object files and library
make re     # Rebuild from scratch
```

## Usage

Include the header and link the library in your project:

```c
#include "libft.h"
```

```bash
gcc your_file.c -L. -lft -o your_program
```

## Project Structure

```
libft/
├── Makefile
├── libft.h
├── ft_*.c       # Standard function implementations
└── ft_lst*.c    # Bonus linked list functions
```

## Notes

- All functions are prefixed with `ft_` to avoid conflicts with standard library names.
- No standard library functions are used in the implementations (except where explicitly allowed).
- Memory management follows strict no-leak policies. 
