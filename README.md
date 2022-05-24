# 42_libft
Libft is an individual project at 42 that requires us to re-create some standard C library functions including some additional ones that can be used later to build a library of useful functions for the rest of the program.

Disclaimer: Reinventing the wheel is bad, 42 makes us do this just so we can have a deeper understanding of data structures and basic algorithms. At 42 we're not allowed to use some standard libraries on our projects, so we have to keep growing this library with our own functions as we go farther in the program.

| Basic Functions| String Functions| Memory Functions| Extra Functions| File Functions | List Functions |
| -------------  | --------------- | --------------- | -------------  | -------------  | -------------  |
| ft_isalpha     | ft_strlen       | ft_memcmp       | ft_substr      | ft_putchar_fd  | ft_lstnew      |
| ft_isdigit     | ft_strchr       | ft_memset       | ft_strjoin     | ft_putstr_fd   | ft_lstadd_front|
| ft_isalnum     | ft_strrchr      | ft_memmove      | ft_strtrim     | ft_putendl_fd  | ft_strtrim     |
| ft_isascii     | ft_strncmp      | ft_memchr       | ft_split       | ft_putnbr_fd   | ft_lstsize     |
| ft_isprint     | ft_strlcpy      | ft_memcpy       | ft_itoa        | ft_memcpy      | ft_lstlast     |
| ft_toupper     | ft_strlcat      | ft_calloc       | ft_strmapi     | ft_calloc      | ft_lstadd_back |
| ft_tolower     | ft_strnstr      |                 | ft_striteri    |                | ft_lstdelone   |
|                |                 |                 |                |                |ft_lstclear     |
|                |                 |                 |                |                |ft_lstiter      |
|                |                 |                 |                |                |ft_lstmap       |

# Content of List(Struct)
```
typedef struct s_list {
void *content;
struct s_list *next; 
} t_list;
```
void \*content
> The data contained in the node that allows to store any kind of data.

struct s_list \*next
> The address of the next node, or NULL if the next node is the last one.
