# 🖨️ ft_printf - 42 School Project

**ft_printf** is a C project from **42 School** where you reimplement the standard `printf` function from `<stdio.h>`.  
The goal is to understand **variable arguments**, **format specifiers**, and advanced string formatting in C.

---

## 🎯 Project Goals

- Reproduce the behavior of the standard `printf` function.  
- Handle **conversion specifiers**, **flags**, **width**, **precision**, and **length modifiers**.  
- Work with **variable arguments** using `stdarg.h`.  
- Learn proper memory management and error handling in C.  

---

## 📚 Features Implemented

The project supports the following conversion specifiers:

| Specifier | Description                   |
|-----------|-------------------------------|
| `%c`      | Print a character             |
| `%s`      | Print a string                |
| `%p`      | Print a pointer address       |
| `%d`, `%i`| Print a signed decimal number|
| `%u`      | Print an unsigned decimal number |
| `%x`      | Print a number in hexadecimal (lowercase) |
| `%X`      | Print a number in hexadecimal (uppercase) |
| `%%`      | Print a literal percent sign  |

**Flags supported:**

- `-` : left-justify  
- `0` : pad with zeros  
- Width and precision modifiers  

---

## 📁 Project Structure

ft_printf/
├── includes/
│ └── ft_printf.h # Header file with function prototypes
├── srcs/
│ ├── ft_printf.c # Main ft_printf function
│ ├── utils.c # Helper functions
│ ├── print_char.c # Character printing
│ ├── print_str.c # String printing
│ ├── print_int.c # Integer printing
│ └── print_hex.c # Hexadecimal printing
├── Makefile # Build library
└── README.md


---

## ⚙️ Compilation

To compile the library:

```bash
make
make clean (rm *.o)
make fclean (rm *.o && rm printflibft.a)
make re (make fclean && make)
