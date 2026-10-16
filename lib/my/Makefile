ifeq ($(OS),Windows_NT)
    RM = del /F /Q
    FIXPATH = $(subst /,\,$1)
else
    RM = rm -f
    FIXPATH = $1
endif

NAME = libmy.a
SRC  = $(wildcard *.c)
OBJ  = $(SRC:.c=.o)

all: $(NAME)

$(NAME): $(OBJ)
	ar rcs $(NAME) $(OBJ)

%.o: %.c
	gcc -Wall -Wextra -Werror -c $< -o $@

clean:
	$(RM) $(call FIXPATH,$(OBJ))

fclean: clean
	$(RM) $(call FIXPATH,$(NAME))

re: fclean all

.PHONY: all clean fclean re
