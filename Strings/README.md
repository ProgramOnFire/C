Immutable string<br>
char * str1 = "Hello";<br>
str1[0] = 'J';  // this would crash<br>

Mutable string<br>
char str[] = "Hello World\n";<br>
This code behaves exactly as if we wrote:<br>
char str[] = {'H', 'e', 'l', 'l', 'o', ' ','W', 'o', 'r', 'l'  'd', '\n', '\0'};<br>

To compare string using strcmp in string.h library:<br>
Returns 0 if strings are equal else return non zero.<br>
It returns a positive number if the first string is “greater than” the second string and a negative number if the first string is “less than” the second string.<br>
Here “greater than” and “less than” refer to lexicographic order —what you would think of as “alphabetical ordering,” but extended to encompass the fact that strings may have non-letters. The comparison is case sensitive (so abc is different from Abc), but there is another function, strcasecmp which performs case-insensitive comparison.<br>
Syntax: int strcmp(const char *leftStr, const char *rightStr );<br>

strlen()<br>
syntax: int strlen(const char *string);<br>
strlen() function doesn't count the null character \0 while calculating the length.<br>

strcpy()<br>
We can easily copy pointer to string but not the case in 2 array.<br>
syntax: char* strcpy(char* destination, const char* source);<br>
The strcpy() function copies the string pointed by source (including the null character) to the destination.<br>
The strcpy() function also returns the copied string.<br>
When you use strcpy(), the size of the destination string should be large enough to store the copied string. Otherwise, it may result in undefined behavior.<br>

strdup()<br>
Syntax : char *strdup(const char *s);<br>
This function returns a pointer to a null-terminated byte string, which is a duplicate of the string pointed to by s. The memory obtained is done dynamically using malloc and hence it can be freed using free().<br>
It returns a pointer to the duplicated string s.<br>

memcpy():<br>
// Copies "numBytes" bytes from address "from" to address "to"<br>
void * memcpy(void *to, const void *from, size_t numBytes);<br>
1) memcpy() doesn’t check for overflow or \0<br>
2) memcpy() leads to problems when source and destination addresses overlap.<br>

memmove():<br>
memmove() is used to copy a block of memory from a location to another. It is declared in string.h<br>
// Copies "numBytes" bytes from address "from" to address "to"<br>
void * memmove(void *to, const void *from, size_t numBytes);<br>
memcpy() simply copies data one by one from one location to another. On the other hand memmove() copies the data first to an intermediate buffer, then from buffer to destination.<br>

string to interger using atoi()<br>
The C library function int atoi(const char *str) converts the string argument str to an integer (type int).<br>
