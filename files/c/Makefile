##
## EPITECH PROJECT, 2022
## Makefile
## File description:
## jitter jitter
##

SRC	=	./hello_world.c	\

OBJ	=	$(SRC:.c=.o)

REM	=	*.gcno	\
		*.gcda

CC	=	gcc

CFLAGS	=	-Wall -Wextra

CPPFLAGS	=	-I./include

NAME	=	"hw.out"

all:	$(NAME)

$(NAME):	$(OBJ)
	$(CC) -o $(NAME) $(OBJ) $(CFLAGS) $(CPPFLAGS)

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(NAME)
	rm unit_tests

re: fclean all clean

.PHONY: fclean all clean re

