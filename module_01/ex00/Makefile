# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: gborne <gborne@student.42.fr>              +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/05/19 14:53:10 by gborne            #+#    #+#              #
#    Updated: 2022/05/29 15:04:43 by gborne           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

SRCS			= main.cpp Zombie.cpp newZombie.cpp randomChump.cpp
OBJS			= $(SRCS:.cpp=.o)

CXX				= g++
RM				= rm -f
CXXFLAGS		= -Wall -Wextra -Werror -std=c++98

NAME			= zombie

all:			$(NAME)

$(NAME):		$(OBJS)
				$(CXX) $(CXXFLAGS) -o $(NAME) $(OBJS)

clean:
				$(RM) $(OBJS)

fclean:			clean
				$(RM) $(NAME)

re:				fclean $(NAME)

test:			$(NAME)
				./megaphone "shhhhh... I think the students are asleep..."
				./megaphone Damnit " ! " "Sorry students, I thought this thing was off."
				./megaphone

.PHONY:			all clean fclean re test
