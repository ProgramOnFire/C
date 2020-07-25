If we wanted to declare an array of 4 ints called myArray, we would write:<br>
int myArray[4];<br>

Initializing:<br>
int myArray[4] = {42, 39, 16, 7};<br>
int myArray[4] = {0}; // initialize all elements to<br>
int myArray[] = {42, 39, 16, 7}; // compiler figures out [4]<br>

We’ll also note that you can use a similar syntax to initialize structs. For example, the following will initialize the first field of p to 3 and the second field to 4:<br>
point p = {3, 4};<br>

for structs, this form of initialization is very brittle–if you add another field to the struct before or in between these two, you will no longer be initializing the fields the way you intend.<br>
point p = { .x = 3, .y = 4};<br>

If you are initializing an array of structs, these two techniques work particularly well together (an example of composability ). For example, we could declare and initialize an array of three points:<br>
point myPoints[] = { {.x = 3, .y = 4},
                     {.x = 5, .y = 7},
                     {.x = 9, .y = 2} };
