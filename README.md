# Libmy

This project is a libmy that will recreate some functions of the libc and also some utility functions.

## Compiling

To create the `libmy.a`, you need to use the `Makefile` in the `lib/my` folder.

| Command       | Action                                      |
| ------------- | ------------------------------------------- |
| `make`        | Compile the lib and create `libmy.a`        |
| `make clean`  | Delete all the `.o` files                   |
| `make fclean` | Delete all the `.o` files and the `libmy.a` |
| `make re`     | Rebuild the whole lib                       |

## Current functions

- [x] void my_putchar(char c);
- [x] int my_putstr(char const \*str);
- [x] int my_put_nbr(int nb);
- [ ] int my_showstr(char const \*str);
