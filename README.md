# C

#include <stdio.h>#header files

int main(){
printf("C");
return 0;
} #body
#semicolon is expected after evry state ment
to comment// is used


#on printing return 0  statement control is tansferred out of the main function &program will execute this code
#hello world
#main function is the starting point of the c program is mandatory




#include<stdio.h>
int main(){
   printf("hello world")    ;

return 0;
}
/*multiline comment */
any valid alphabet symbool ,digit is termed as character in c
#variable is a way to store information
it can be formed from any combination ofvalid alphabets,digits and special symbol
its an entiy whose value may or maynot change
cnstant is whose valueemain same (3,10 etc)
keyword we cannnot change the meaning of the world
#variable=first character of variable is alphabet or underscore no comma ,space, sspecial character, key word allowed

#DATA TYPES

EACH VARIABLE IS RELATEED TO DIFFERENT TO DIFFERENT DATA TYPE WHICH ALLOCATE DIFFERENT AMOUNT OF MEMORY 
DATA TYPES IN C PRORAMMING HAS
RANGE OF DATA
TYPE OF DATA STRED
NO OF BYTES OCCUPIED IN MEMORY

PRIMITIVE:-
INT ,FOAT ,DOUBLE,CHAR
DERIVED :-ARRAY,STRUCTURE,UNION,POINTER,ENUM
INT,FLOAT OCCUPIES 4 BYTES OF MEMORY
DOUBLE OCCUPIES 8 BYTE 
CHAR OCCUPIES 1 BYTE
#HOW TO DECLARE A VARIABLE
<DATA_TYPE>VARIABLE_NAME;
int amount=9000;
format specifier %d-int
%f-float
%lf-double
%c-character
%s-string
char alpha='e'
printf("%d %c",amount,alpha)
\n for next line
