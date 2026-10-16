CC	=	gcc
AR	=	ar rcs
RM	=	rm -f
NAME	=	libmy.a
# SRC have nothing for now
OBJ	=	$(SRC:.c=.o)
CFLAGS	=	-Wall -Wextra	-Werror

all:	$(NAME)

$(NAME): $(OBJ)
	$(AR) $(NAME) $(OBJ)

clean:
	$(RM) $(OBJ)

fclean: clean
	$(RM) $(NAME)

re: fclean all

.PHONY: all clean fclean re
