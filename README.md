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



#SWITCH

switch(expression)(exxpression can be anything that evaluates to integer value or a character constant. it can't be float,double,string)
{case value1:
/*block of code*/
break;
case value2:
/*block of code*/
break;
case value3:
/*block of code*/
break;
case value4:
/*block of code*/
break;
default:
/*block of code*/
}


#include<stdio.h>
int main(){
int choice=3;
switch(choice)//(exxpression can be anything that evaluates to integer value or a character constant. it can't be float,double,string)
{case 1:
/*block of code*/
printf("the value is value1");
break;
case 2:
/*block of code*/
printf("the value is value 2");
break;
case 3:
/*block of code*/
printf("the value is value 3");
break;
case 4:
/*block of code*/
printf("the value is value 4");
break;
default:
/*block of code*/
printf("no value");
}
}
#EXAMPLE
#include<stdio.h>
int main(){
int choice=3;
switch(choice)//(exxpression can be anything that evaluates to integer value or a character constant. it can't be float,double,string)
{case 1:
/*block of code*/
printf("the value is value1");
break;
case 2:
/*block of code*/
printf("the value is value 2");
break;
case 3:
/*block of code*/
printf("the value is value 3");
break;
case 4:
/*block of code*/
printf("the value is value 4");
break;
default:
/*block of code*/
printf("no value");
}
}

#GOTO


int main(){

 line 1;
 line 2;
 goto label;
 line 3 ;
 line 4;
 label:
 line 5;
 line 6;
 return 0;
 }



#include<stdio.h>
int main(){printf("the printf value is 0");
printf("the printf value is 1");
printf("the printf value is 2");
goto skip;
printf("the printf value is 3");
printf("the printf value is 4");
skip:
printf("the printf value is 5");

           }



#while loop in c programming
while(condition)
{
#block of code;
}

#include<stdio.h>
int main(){int count=0;
while(count<2)
{
    count=count+1;
    printf("%d",count);
}
printf("end of while");
}



while(1)
{printf("print the while loop");
}

#for infinite times as 1 will always be true 




#write the code for sum of numbers
#include<stdio.h>
int main(){int count;
int n=0;
int a=0;
int temp;
scanf("%d",&count);
while(n<=count)
{
    a=a+n;
     n=n+1;
}
printf("%d",a);
}


#do while


do{
//block of statement
}while(condition);

#in here bloc of coode is run atleast once before making a condition evaluation 
#include<stdio.h>
int main(){
int n=0;
int count=20;
do
{
    n=n+1;
    printf("\%d",n);


}while(n<=count);
}


#for loop
for(initialization;condition;increment/decrement)
{
}

#include<stdio.h>
int main(){
for (int i=0;i<2;i++)
{
    printf("%d",i);
}
}

#include<stdio.h>
int main(){int a=0;
for (int i=0;i<=10;i++)
{    a=a+i;
}
 printf("%d",a);
}


fibonaci series
#include<stdio.h>
int main(){int a=0;
int b=1;
int c;
int n;
scanf("%d",&n);
printf("%d %d",a,b);
for (int i=2;i<n;i++)
 {
         c=a+b;
         a=b;
         b=c;
         printf("%d",c);

 }


#break


#include<stdio.h>
int main(){int a=0;
int b=1;
int c;
int n;
scanf("%d",&n);
printf("%d %d",a,b);
for (int i=2;i<n;i++)
 {
         c=a+b;
         a=b;
         b=c;
         printf("%d",c);
      if (i==5)
      {
          break;
      }
 }
printf("end is 5");
}

#break basically terminat the loop statement

#continue it will skip the following lines of code and force the next iteration of the loop.

#include<stdio.h>
int main(){int a=0;
int b=1;
int c;
int n;
scanf("%d",&n);
printf("%d %d",a,b);
for (int i=2;i<n;i++)
 { if (i==5)
      {
          continue;
      }
         c=a+b;
         a=b;
         b=c;
         printf("%d",c);

 }
printf("end is 5");
}

#to make*
        * *
        * * *
        * * * *
        
#include<stdio.h>
int main(){
int n;
int i;
scanf("%d",&n);
for (i=0;i<n;i++)
  {
      printf("\n%c",'*');
      int j=0;

        while(j<i)
    {
        printf("%c",'*');
        j=j+1;

    }
}
}        
