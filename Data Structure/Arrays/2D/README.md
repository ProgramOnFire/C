Initialization of 2D Array<br>
There are two ways to initialize a two Dimensional arrays during declaration.<br>
int disp[2][4] = {<br>
    {10, 11, 12, 13},<br>
    {14, 15, 16, 17}<br>
};<br>
OR<br>
int disp[2][4] = { 10, 11, 12, 13, 14, 15, 16, 17};<br>

Things that you must consider while initializing a 2D array<br>
/* Valid declaration*/<br>
int abc[2][2] = {1, 2, 3 ,4 }  <br>
/* Valid declaration*/ <br>
int abc[][2] = {1, 2, 3 ,4 }  <br>
/* Invalid declaration – you must specify second dimension*/<br>
int abc[][] = {1, 2, 3 ,4 }   <br>
/* Invalid because of the same reason  mentioned above*/<br>
int abc[2][] = {1, 2, 3 ,4 }<br>

while accessing using pointer (or during dynamic initialization) and if p is base address then,<br>
while addressing p+i*columnsize+j
