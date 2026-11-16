*This project has been created as part of the 42 curriculum by **kymuller**.*

# Libft

![https://medium.com/@simonzerisenay/custom-c-library-secure-and-efficient-2e450da1c627](https://miro.medium.com/v2/resize:fit:720/format:webp/1*8lw6KktyFOL3wSCdZSRdsw.jpeg)
---
![https://img.shields.io/badge/42-Common%20Core-000000?style=for-the-badge&logo=42](https://img.shields.io/badge/42-Common%20Core-000000?style=for-the-badge\&logo=42)
![https://img.shields.io/badge/Language-C-blue?style=for-the-badge&logo=c](https://img.shields.io/badge/Language-C-blue?style=for-the-badge\&logo=c)

**Your very first own C library.**

Recreating essential C standard library functions from scratch.

---

## 📖 Description

**Libft** is the first project of the 42 Common Core curriculum.

The goal of this project is to create a personal C library by reproducing several functions from the standard C library and developing additional utility functions.

Instead of relying on existing implementations, every function must be written from scratch, following the constraints and coding standards imposed by 42.

This project provides a solid foundation in C programming and introduces important concepts such as:

- Memory allocation and management.
- Pointers and pointer manipulation.
- String manipulation.
- Data structures.
- Linked lists.
- Defensive programming and error handling.
- Compilation and static libraries.

The final result is a reusable static library named **`libft.a`**, which can be integrated into future C projects.

## 🛠️ Library Overview

Libft is organized into several groups of functions.

### 1. Libc Functions

Reimplementations of standard C library functions.

| Function     | Description                                     |
| ------------ | ----------------------------------------------- |
| `ft_isalpha` | Checks whether a character is alphabetic.       |
| `ft_isdigit` | Checks whether a character is a digit.          |
| `ft_isalnum` | Checks whether a character is alphanumeric.     |
| `ft_isascii` | Checks whether a character belongs to ASCII.    |
| `ft_isprint` | Checks whether a character is printable.        |
| `ft_strlen`  | Calculates the length of a string.              |
| `ft_memset`  | Fills memory with a specified byte.             |
| `ft_bzero`   | Sets a memory area to zero.                     |
| `ft_memcpy`  | Copies memory from one location to another.     |
| `ft_memmove` | Copies memory while handling overlapping areas. |
| `ft_strlcpy` | Copies a string with size limitation.           |
| `ft_strlcat` | Concatenates strings with size limitation.      |
| `ft_toupper` | Converts a character to uppercase.              |
| `ft_tolower` | Converts a character to lowercase.              |
| `ft_strchr`  | Finds the first occurrence of a character.      |
| `ft_strrchr` | Finds the last occurrence of a character.       |
| `ft_strncmp` | Compares two strings up to a given length.      |
| `ft_memchr`  | Searches for a byte in memory.                  |
| `ft_memcmp`  | Compares two memory areas.                      |
| `ft_strnstr` | Searches for a substring.                       |
| `ft_atoi`    | Converts a string into an integer.              |
| `ft_calloc`  | Allocates zero-initialized memory.              |
| `ft_strdup`  | Duplicates a string.                            |

### 2. Additional Functions

Utility functions designed to simplify common string and memory operations.

| Function        | Description                                              |
| --------------- | -------------------------------------------------------- |
| `ft_substr`     | Extracts a substring.                                    |
| `ft_strjoin`    | Concatenates two strings into a new one.                 |
| `ft_strtrim`    | Removes specified characters from both ends of a string. |
| `ft_split`      | Splits a string using a delimiter.                       |
| `ft_itoa`       | Converts an integer into a string.                       |
| `ft_strmapi`    | Applies a function to each character of a string.        |
| `ft_striteri`   | Applies a function to each character using its index.    |
| `ft_putchar_fd` | Writes a character to a file descriptor.                 |
| `ft_putstr_fd`  | Writes a string to a file descriptor.                    |
| `ft_putendl_fd` | Writes a string followed by a newline.                   |
| `ft_putnbr_fd`  | Writes an integer to a file descriptor.                  |

### 3. Linked Lists Functions

This part introduces linked lists and dynamic data structures.

>[!NOTE]
>The library implements a singly linked list using the `t_list` structure.

| Function          | Description                                                |
| ----------------- | ---------------------------------------------------------- |
| `ft_lstnew`       | Creates a new list element.                                |
| `ft_lstadd_front` | Adds an element at the beginning.                          |
| `ft_lstsize`      | Counts the number of elements.                             |
| `ft_lstlast`      | Returns the last element.                                  |
| `ft_lstadd_back`  | Adds an element at the end.                                |
| `ft_lstdelone`    | Deletes one element.                                       |
| `ft_lstclear`     | Deletes an entire list.                                    |
| `ft_lstiter`      | Applies a function to every element.                       |
| `ft_lstmap`       | Creates a new list by applying a function to each element. |

---

## ⚙️ Instructions

### Installation

Clone the repository:

```bash
git clone git@vogsphere.42nice.fr:vogsphere/intra-uuid-51d970e0-5626-4d27-88c0-202ecfb93520-7802420-kymuller
cd libft
```

### Compilation

Compile the mandatory part:

```bash
make
```

Remove object files:

```bash
make clean
```

Remove object files and the library:

```bash
make fclean
```

Recompile everything:

```bash
make re
```

After successful compilation, the static library `libft.a` will be generated at the root of the project.

### Using Libft in another project

Compile the program with a main:

```bash
cc main.c libft.a -o program
```

Run the executable:

```bash
./program
```

---

## 📁 Project Structure

```text
libft/
│
├── Makefile
├── README.md
├── libft.h
│
├── ft_isalpha.c
├── ft_isdigit.c
├── ft_isalnum.c
├── ft_isascii.c
├── ft_isprint.c
├── ft_strlen.c
├── ft_memset.c
├── ft_bzero.c
├── ft_memcpy.c
├── ft_memmove.c
├── ft_strlcpy.c
├── ft_strlcat.c
├── ft_toupper.c
├── ft_tolower.c
├── ft_strchr.c
├── ft_strrchr.c
├── ft_strncmp.c
├── ft_memchr.c
├── ft_memcmp.c
├── ft_strnstr.c
├── ft_atoi.c
├── ft_calloc.c
├── ft_strdup.c
│
├── [Additional functions]
│
└── [Linked list functions]
```

---

## 🧠 Technical Choices

This project focuses on understanding how standard C functions work internally.

Some important technical aspects include:

- **Memory management:** Using `malloc` and `free` correctly to avoid memory leaks.
- **Pointers:** Manipulating memory addresses and passing data efficiently.
- **String handling:** Working with null-terminated strings.
- **Error handling:** Managing invalid inputs and allocation failures.
- **Linked lists:** Implementing dynamic structures using pointers.
- **Code organization:** Separating functions into individual source files and using a shared header.

All functions are designed to respect the 42 Norm and the constraints specified in the project subject.

---

## 📚 Resources

The following resources are useful for understanding and implementing the project:

- [GeeksForGeeks](https://www.geeksforgeeks.org/c/c-programming-language/) – C language documentation.
- [Linux Manual Pages](https://man7.org/linux/man-pages/) – Reference for standard C and system functions.
- [W3School](https://www.w3schools.com/c/) – C programming tutorials.
- [IBM](https://www.ibm.com/docs/fr/ibm-mq/9.3.x?topic=mqi-c-programming) – Additional C programming reference.

### AI Usage

AI tools (ChatGPT) were used as an assistance tool during the preparation of this project's documentation.

Specifically, AI assistance was used for:

- Structuring and formatting the README file.
- Improving the clarity of technical descriptions.

AI was not used as a substitute for understanding the project's implementation. The code, its behavior and its compliance with the 42 requirements remain the responsibility of the author.

---

## 🎯 Learning Outcomes

Through Libft, I developed a better understanding of:

- The fundamentals of C programming.
- Pointer arithmetic and memory manipulation.
- Dynamic memory allocation.
- String and character manipulation.
- The implementation of standard library functions.
- Linked lists and basic data structures.
- Compilation, static libraries and Makefiles.
- Writing clean, structured and reusable code.

Libft is the foundation for many future projects in the 42 Common Core curriculum.

---
