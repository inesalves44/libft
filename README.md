# libft (42 - lvl 0)

## 1. Overview

This project was the first project of the common core in 42 school!

This project has the objective if creating a static library composed of useful functions that will help in the 42 curriculum. 

## 2. The functions

  ### 2.1 Part 1 - Functions of the system
      • isalpha           • toupper
      • isdigit           • tolower
      • isalnum           • strchr
      • isascii           • strrchr
      • isprint           • strncmp
      • strlen            • memchr
      • memset            • memcmp
      • bzero             • strnstr
      • memcpy            • atoi
      • memmove           • calloc
      • strlcpy           • strdup
      • strlcat
      
   ### 2.2 Part 2 - Other useful functions
       * ft_substr - we can get a substring from a given string;
       * ft_strjoin - join two strings;
       * ft_strtrim - trims a given string with a base of another;
       * ft_split - splits a string with a given character, resulting in an array of strings;
       * ft_itoa * transforms an integer to ascii;
       * ft_strmapi - applies a function on each char of a string and creates a new resulting string;
       * ft_striteri - applies a function on each char of a string;
       * ft_putchar_fd - puts a chosen character in an fd;
       * ft_putstr_fd - puts a chosen string in an fd;
       * ft_putendl_fd - puts a chosen string followed by a newline in an fd;
       * ft_putnbr_fd - puts a chosen number in an fd;
       
   ### 2.3 Bonus - Introduction to Linked Lists
In this part we use Linked Lists with this structure:
``` 
typedef struct s_list
{
    void *content;
    struct s_list *next;
}   t_list;
```
Functions:

        * ft_lstnew - create a node;
        * ft_lstadd_front - add a node to the front of the list;
        * ft_lstsize - get the size of a list;
        * ft_lstadd_back - add a node to the back of the list;
        * ft_lstdelone - deletes a node of the list;
        * ft_lstclear - clears a node and the next nodes;
        * ft_lstiter - applies a function to each node of a list;
        * ft_lstmap - applies a function to each node of a list and creates a new list;
        * ft_lstlast - returns the last node;
        
 ## 3. Make Commands
```
make all - creates the library
make bonus - creates the library for bonus
make clean - cleans the objects
make fclean - cleans the library, also runs clean
make re - runs clean and fclean and then runs all 
make rebonus - runs clean and fclean and then runs bonus
 ```
As stated above this project creates a library. This library is composed of object files that then are used in the linker fase of a compilation.

Basically to use the library you compile it like this:
```
cc -Wall -Werror -Wextra your_file.c libft.a
```

Thank you for reading!
slack: idias-al
