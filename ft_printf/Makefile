
CC = gcc

CFLAG = -Wall -Wextra -Werror -g

NAME = libftprintf.a

SRCDIR = ./src

SRC = flag.c			\
      ft_parsing.c		\
      init.c			\
      ft_printf.c		\
      tools.c			\
      ft_space.c        \
      ft_spec.c			\
      ft_specif_nb.c    \
      ft_spec_bonus.c   \
      ft_specif_o.c		\
      ft_spec_l.c       \
      ft_spec_ld.c      \
      ft_itoamax.c      \
      ldtoa.c           \
      fc_norm.c         \
      ft_norm.c			\
      get_type.c        \
      ft_strrevchr.c    \
      ft_bonus_color.c  \
      ft_putchar.c		\
      ft_putstr.c		\
      ft_strcmp.c		\
      ft_strlen.c		\
      ft_swap.c			\
      ft_atoi.c			\
      ft_memset.c		\
      ft_bzero.c		\
      ft_memcpy.c		\
      ft_memccpy.c		\
      ft_strdup.c		\
      ft_memmove.c		\
      ft_memchr.c		\
      ft_memcmp.c		\
      ft_strcpy.c		\
      ft_strncpy.c		\
      ft_isalpha.c		\
      ft_isupper.c		\
      ft_islower.c		\
      ft_isdigit.c		\
      ft_isalnum.c		\
      ft_isascii.c		\
      ft_isprint.c		\
      ft_tolower.c		\
      ft_toupper.c		\
      ft_strcat.c		\
      ft_strncat.c		\
      ft_strlcat.c		\
      ft_strchr.c		\
      ft_strrchr.c		\
      ft_strstr.c		\
      ft_strncmp.c		\
      ft_strclr.c		\
      ft_memalloc.c		\
      ft_strdel.c		\
      ft_memdel.c		\
      ft_strmapi.c		\
      ft_striter.c		\
      ft_striteri.c		\
      ft_strnew.c		\
      ft_strmap.c		\
      ft_strequ.c		\
      ft_putnbr.c		\
      ft_putnbr_fd.c	\
      ft_putchar_fd.c	\
      ft_putstr_fd.c	\
      ft_putendl_fd.c	\
      ft_putendl.c		\
      ft_strnequ.c		\
      ft_strsub.c		\
      ft_strjoin.c		\
      ft_strjoin_free.c	\
      ft_strtrim.c		\
      ft_itoa.c			\
      ft_strsplit.c		\
      ft_lstnew.c		\
      ft_memdup.c		\
      ft_putnchar.c		\
      ft_lstadd.c		\
      ft_lstiter.c		\
      ft_lstmap.c		\
      ft_lstdelone.c	\
      ft_lstdel.c		\

OBJ = $(addprefix $(SRCDIR)/,$(SRC:.c=.o))

$(NAME): $(OBJ)
	@ar rc $(NAME) $(OBJ)

all: $(NAME)

test:
	@$(CC) $(NAME) main.c -g -o test_printf

clean:
	@rm -f $(OBJ)

fclean:	clean
	@rm -f $(NAME)

re: fclean all

$(SRCDIR)/%.o : $(SRCDIR)/%.c
	@$(CC) $(CFLAG) -c -o $@ $<

.PHONY : test all re clean fclean
