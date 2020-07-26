Immutable string
char * str1 = "Hello";
str1[0] = 'J';  // this would crash

Mutable string
char str[] = "Hello World\n";
This code behaves exactly as if we wrote:
char str[] = {'H', 'e', 'l', 'l', 'o', ' ','W', 'o', 'r', 'l'  'd', '\n', '\0'};

To compare string using strcmp in string.h library:
Returns 0 if strings are equal else return non zero.
It returns a positive number if the first string is “greater than” the second string and a negative number if the first string is “less than” the second string.
Here “greater than” and “less than” refer to lexicographic order —what you would think of as “alphabetical ordering,” but extended to encompass the fact that strings may have non-letters. The comparison is case sensitive (so abc is different from Abc), but there is another function, strcasecmp which performs case-insensitive comparison.
Syntax: int strcmp(const char *leftStr, const char *rightStr );

strlen()
syntax: int strlen(const char *string);
strlen() function doesn't count the null character \0 while calculating the length.

strcpy()
We can easily copy pointer to string but not the case in 2 array.
syntax: char* strcpy(char* destination, const char* source);
The strcpy() function copies the string pointed by source (including the null character) to the destination.
The strcpy() function also returns the copied string.
When you use strcpy(), the size of the destination string should be large enough to store the copied string. Otherwise, it may result in undefined behavior.

strdup()
Syntax : char *strdup(const char *s);
This function returns a pointer to a null-terminated byte string, which is a duplicate of the string pointed to by s. The memory obtained is done dynamically using malloc and hence it can be freed using free().
It returns a pointer to the duplicated string s.

memcpy():
// Copies "numBytes" bytes from address "from" to address "to"
void * memcpy(void *to, const void *from, size_t numBytes);
1) memcpy() doesn’t check for overflow or \0
2) memcpy() leads to problems when source and destination addresses overlap.

memmove():
memmove() is used to copy a block of memory from a location to another. It is declared in string.h
// Copies "numBytes" bytes from address "from" to address "to"
void * memmove(void *to, const void *from, size_t numBytes);
memcpy() simply copies data one by one from one location to another. On the other hand memmove() copies the data first to an intermediate buffer, then from buffer to destination.

