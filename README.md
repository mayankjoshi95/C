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
INT ,FLOAT ,DOUBLE,CHAR
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


#MODIFIERS IN C


MODIFIERS ARE USED TO MODIFY THE AMOUNT OF STORAGE SPACE ALLOCATED TO A VARIABLE
SAY FOR INT GNU COMPILER GIVES 4 BYTES OF MMORY I CAN TELL THE COMPILER TO GIVE 2 BYTES OF MEMORY
1.SHORT(INT)(4 TO 2 BYTES) 2.LONG(INT(,DOUBLE(8 TO 12 BYTES) 3.SIGNED(INT,CHAR)(VARIABLE ALLOWED TO STORE POSITIVE AND NEAGATIVE VALUES SIGNED INT COUNT ;COUNT=-5) 4.UNSIGNED(INT,CHAR)

BY DEFAULT INT IS SIGNED INT
CHAR IS SIGNED OR UNSIGNED DEPENDING ON WHAT WE PROVIDE IT
#minimum and maximum velue range of the data type
library are <limits.h>
<float.h>


#include<stdio.h>
#include<limits.h>
#include<float.h>
int main(){

double date=1.3;

int age=10;

float amount=12.65;
char alpha='s';

printf("%lf %f %d %c %d %d %d ", date, amount, age,alpha,sizeof(int),INT_MIN,INT_MAX);
printf("%lf %f %d %c %d %d %d %le %le%d %d  %d %d %d %d ", date, amount, age,alpha,sizeof(int),INT_MIN,INT_MAX,FLT_MIN,FLT_MAX,CHAR_MIN,CHAR_MAX,SCHAR_MIN,SCHAR_MAX,UCHAR_MAX);
printf("%le %le",DBL_MIN,DBL_MAX);
return 0;

}




#float and double

#float allow 6 digits after decimal points
#double allow 15 digits after decimal points

float amount=12.65435643;
printf("%0.3f",amount);
(it means only 3 numbers after decimal)
(by default printf display only upto 6 decimal point thus we have to add %.15lf for higher decimal point)

#scanf
scanf("%d",&a)

count=10;
total=++count(first increment count then stor it in total )
totla=count+=(first put the value of the the count in the total then incremnt the count)



#assignment (=,+=,-=,*=,/=,%=)
#relational (>=,<=,>,<,==,!=)
#logical operator(&&,||,!)


#control statement
#if else statement
#include<stdio.h>
int main(){char name ;
int num 1;
int num2;
 scanf("%c",&name);
 scanf("%d",&num1);
 scanf("%d",&num2);
 if (name=='a'){
 printf("%d",num1+num2);
 }
 else{ 
    if (name=='s')
    {printf("%d",num1-num2);
    }
    else{
          if (name=='m')
          {printf("%d",num1*num2);
           }
           else{if (name=='d')
               {printf("%d",num1/num2);
               }
         } 
      }
   }   
         
 
 
 
 }

