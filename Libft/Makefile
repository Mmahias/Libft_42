# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: mmahias <mmahias@student.42.fr>            +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2021/01/05 15:24:30 by mmahias           #+#    #+#              #
#    Updated: 2021/01/05 15:24:35 by mmahias          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #


SRCS	= ft_memset.c ft_bzero.c ft_memcpy.c ft_memccpy.c ft_memmove.c ft_memchr.c ft_memcmp.c ft_strlen.c ft_isalpha.c ft_isdigit.c ft_isalnum.c ft_isascii.c ft_isprint.c ft_toupper.c ft_tolower.c ft_strchr.c ft_strrchr.c ft_strncmp.c ft_strlcpy.c ft_strlcat.c ft_strnstr.c ft_atoi.c ft_calloc.c ft_strdup.c ft_substr.c ft_strjoin.c ft_strtrim.c ft_split.c ft_itoa.c ft_strmapi.c ft_putchar_fd.c ft_putstr_fd.c ft_putendl_fd.c ft_putnbr_fd.c

OBJS	= ${SRCS:.c=.o}

OBJS_BONUS = ${SRCS_BONUS:.c=.o}

NAME	= libft.a

CC	= gcc

CFLAGS	= -Wall -Werror -Wextra -I.

RM	= rm -f

.c.o: 
	  ${CC} ${CFLAGS} -c $< -o ${<:.c=.o}

$(NAME):  ${OBJS}
	  ar -rcs ${NAME} ${OBJS}

all:      ${NAME}

bonus:	${OBJS_BONUS} ${OBJS}
	ar -rcs	${NAME} ${OBJS_BONUS} ${OBJS}

clean:
	  ${RM} ${OBJS} ${OBJS_BONUS}

fclean:	  clean
	  ${RM} ${NAME}

re:	  fclean all

.PHONY:   all clean fclean re
