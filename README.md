

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


#FUNCTIONS


void fname()(void means this function will not return any data)
{

}


#include<stdio.h>
void addition()
{
   int n;
int i;
scanf("%d",&n);
for (i=0;i<=n;i++)
  {

      int j=0;

        while(j<i)
    {
        printf("%c",'*');
        j=j+1;

    }
      printf("\n");

 }
}
int main(){
addition();
}





#factorial
#include<stdio.h>
int n=1;
int nu;
void factorial(nu)
{
    for(int i=1 ;i<=nu;i++)
    {
         n=n*i;
    }
    printf("%d",n)  ;

}


int main(){
    printf("write a number to get the factorial of");
    scanf("%d",&nu);
factorial(nu);
}






#function which return a value

datatype fname(datatype1,datatype2,datatype3,datatype4)
{return  value;
}
int main()
{dataype var=fname(datatype1,datatype2,datatype3,datatype4)
}



#to find the average
#include<stdio.h>

float avg (float nu,float n)

{
float value=(nu+n)/2.0;
return value;
}


int main(){

float c=avg(5,6);
printf("the average value is");

printf("%f",c);
return 0;
}


#FUNCTION PROTOTYPE(simply a declaration of the function that specifies function name parameters and return type.)


#include<stdio.h>


float avg (float nu,float n)
int main(){

float c=avg(5,6);
printf("the average value is");

printf("%f",c);
return 0;
}
float avg (float nu,float n)

{
float value=(nu+n)/2.0;
return value;
}


##IT LEADS TO ERROR I CAN TELL COMPILER THAT I WILL BE DEFINING FUNCTION SOMEWHERE ELSE IN THE CODE.


#scope of variable  in c


#include<stdio.h>


float avg (float nu,float n);
int main(){

float c=avg(5,6);
printf("the average value is");

printf("%f",value);
return 0;
}
float avg (float nu,float n)

{
float value=(nu+n)/2.0;
return value;
}
#here value has the local scope thus it can't be run 

#scope of variable value is local to the main fnction and it is not aaccesible to the main function.



#include<stdio.h>


float avg (float nu,float n);
int value=1000;
int main(){

float c=avg(5,6);
printf("the average value is");

printf("the value in global%d",value);
return 0;
}
float avg (float nu,float n)

{
float value=(nu+n)/2.0;
printf("the value in local%f",value);
return value;
}

#here value is defined for both global and for local 


##AN ARRAY IS A COLLECTIVE NAME GIVEN TO A GROUP OF VARIABLES OR CONSTANT VALUES OF SAME TYPES.

#HERE INDEX START WITH THE ZERO



#SYNTAX TO DECLARE A 1-D ARRAY


datatype  arraryname[number of elements];

float avg[5]={1.2,1.2,1.4,1.5,1.7};


#include<stdio.h>
int main(){
    float amount[5]={1.1,2.3,2.3,4.3,5.4};
    printf("%f",amount[2]);
}

#another way of defining array


#include<stdio.h>
int main(){
    float amount[5];
    amount[0]=1.2;
    amount[1]=1.3;
    amount[2]=1.4;
    amount[3]=1.6;
    amount[4]=1.8;
    amount[5]=2.9;

    printf("%f",amount[2]);
}



#this is called dynamic allocation of an array


#include<stdio.h>
int main(){
    float amount[]={1.1,1.2,3.4,4.5,3.6};

    printf("%f",amount[2]);
}

#accept a multiple values  as an input  from the user and store it in an array

#include<stdio.h>
int main(){
    float amount[10];
    for (int i=0;i<10;i++)
        scanf("%f",&amount[i]);
    for (int i=0;i<10;i++)
        printf("%f",amount[i]);
}



#to find the average




#include<stdio.h>
float sum=0;
int main(){
    float amount[5];
    for (int i=0;i<5;i++)
    {scanf("%f",&amount[i]);}
    for (int i=0;i<5;i++)
       {sum+=amount[i];
         printf("%f",sum);}
    printf("\n the average is %f",sum/5.0);
}


##2D array in C


datatype arrayname[row][column];


#include<stdio.h>
int main()
{
    int count[2][3]={10,20,30,40,50,60};(10,20,30 are stored in one row and 40,50,60 in other row)
    return 0;
}


#include<stdio.h>
int main()
{
    int count[2][3]={10,20,30,40,50,60};
     for (int i=0;i<2;i++)
     {
         for (int j=0;j<3;j++)
         {
             printf("%d",count[i][j]);
         }
         printf("\n");
     }
    return 0;
}


#include<stdio.h>
int main()
{
    int count[2][3];
     for (int i=0;i<2;i++)
     {
         for (int j=0;j<3;j++)
         {
             scanf("%d",&count[i][j]);
         }
         printf("\n");
     }
     for (int i=0;i<2;i++)
     {
         for (int j=0;j<3;j++)
         {


     printf("%d",count[i][j]);
     }
     printf("\n");
     }
    return 0;
}



##2 2D 3*3 matrix sum

#include<stdio.h>
int main()
{
    int count[3][3];
     for (int i=0;i<3;i++)
     {
         for (int j=0;j<3;j++)
         {
             scanf("%d",&count[i][j]);
         }
         printf("\n");
     }
     int counts[3][3];
     for (int i=0;i<3;i++)
     {
         for (int j=0;j<3;j++)
         {
             scanf("%d",&counts[i][j]);
         }
         printf("\n");
     }
     int sum[3][3];
     for (int i=0;i<3;i++)
     {
         for (int j=0;j<3;j++)
         {
          sum[i][j]=count[i][j]+counts[i][j];
     }
     printf("\n");
     }
     for (int i=0;i<3;i++)
     {
         for (int j=0;j<3;j++)
         {
             printf("%d",sum[i][j]);
         }
         printf("\n");
     }
    return 0;
}




#POINTER IN C

POINTER IS A VARIABLE THAT POINTS TO AN ADDRESS OF A VARIABLE
#&IS USED TO GET AN ADDRESS
#&count wil return address of variable count 
#include <stdio.h>
int main(){int count;
count=25;
printf("%x",&count);}
#it will return address of the count and variable count is stored at that address inside the memory

#DECLARE A POINTER VARIABLE

datatype *pointer_name(if my pointer variable is pointing to an int data type datattype is int).
#include <stdio.h>
int main(){int count;
count=25;
int *pointer;//pointer will point to an address

printf("%x",&count);
pointer=&count;
printf("\n%x",pointer);
printf("%d",*pointer);//*pointer is read as content at pointer i.e content at address pointer is pointing to
printf("%d",*(&count);}//  content at address of count


#change the value using pointer .



#include <stdio.h>
int main(){int count;
count=25;
int sum=30;
int *pointer;//pointer will point to an address
int *sumpointer;
sumpointer=&sum;
printf("%x",&count);
pointer=&count;
printf("\n%x",pointer);
printf("%d",*pointer);//*pointer is read as content at pointer}
printf("%x",sumpointer);
sumpointer=pointer;
printf("%d",*sumpointer);
}


#addition,subtraction of two pointer is not allowed in C
#count==sum this can be done it gives the ouput 0 or 1


##use of pointer
#include<stdio.h>
void display(int *ptr)
{
    printf("value entered by the user is %d",*ptr);
}
int main(){
    int n=90;
    int *num;
    num=&n;
    display(num);


}




##SUM USING POINTER
#include<stdio.h>
void display(int *ptr,int*pt)
{
    printf("sum by the user is %d",*ptr+*pt);
}
int main(){
    int n;
    int m;
    scanf("%d",&n);
    scanf("%d",&m);
    int *num;
    int *nu;
    num=&n;
    nu=&m;

    display(num,nu);


}





##STRING 


#A STRING IS A SDDRIES OF CHARACTER  IN AGROUP THAT OCCUPY CONTAGIOUS MEMORY.
#A STRING IN CIS AN ARRAY OF CHARACTERS
#A GROUP OF CHARACTERS INCLUDING ALPHABETS,DIGITS,AND SPECIAL SYMBOL IS CALLED STRING.


#include <stdio.h>
int main(){char a[20]="programming"
char *a="programming";
            printf(a);}



#include <stdio.h>
int main(){char a[20]="prrogramming";
            printf("%s",a);}

#include <stdio.h>
int main(){char *a="prrogramming";
            printf("%s",&a[0]);}


#include <stdio.h>
int main(){char *a="prrogramming";
            puts(a);}
            
            ######scanf will never worl if the input entered by the user has spaccee in it.
            ######thus fgets is used .fgets(comments,5,stdin)#for example number of character is 4 then buffer size is 5
            #buffer size greater than number of characters that needs to be accepted.
            
            
 #include <stdio.h>
int main(){

    char comment[20] ;
    printf("enter a text  ");
    scanf("%s",&comment);
    printf("\n text entered by the user is %s",comment);
    return 0;

}
##fgets
#include <stdio.h>
int main(){

    char comment[20] ;
    printf("enter a text  ");
    fgets(comment,5,stdin);
    printf("\n text entered by the user is %s",comment);
    return 0;

}

#TO FIND THE LENGTH OF THE STRING

#include <stdio.h>
int main(){
     int n=999;
     int length=0;
    char comment[n];
    printf("enter a text  ");
    fgets(comment,n+1,stdin);
    for(int i=0;comment[i]!='\n';i++)
    {
        length=length+1;
    }
    printf("\n text entered by the user is %d",length);
    return 0;

}


#include <stdio.h>
int main(int argc,const char * argv[]){
    char comment1[]="this is my first comment";
    printf("length of the string  %d",strlen(comment1));//copy the length
    char destination[100];
    strcpy(destination,comment1);//copy the string
    printf("destination is %s",destination);
    char destination1[100];
    strncpy(destination1,comment1,3);//first intial n character
    printf("%s",destination1);
    strcat(destination1,comment1);//concatinate the string
    printf("%s",destination1);
    strncat(destination1,comment1,3);//concatenate leftmost comment1 with destination1
    printf("%s",destination1);
    strcmp(destination1,comment1);//if 1st=2nd return 0,if 1st>2nd return 1,1st<2nd return -1;

    int length=strlen(comment1);//for reversing the string
    for (int i=length-1;i>=0;i--)
    {
        printf("%c",comment1[i]);
    }
    return 0;

}




#STRUCTURES IN C

STRUCTURE IS A SPECIAL TYPE OF C DATATYPE IT ALLOWS MULTIPLE STRUCTURES TO BE GROUPED TOGETHER
##BASICALLY STRUCTURE " ANIMAL" CAN BE CONSIDERED  AS A COLLECTION OF PROPERTIES .
##"ANIMAL HAS THE FOLLOWING PROPERTIES:
##AGE ,GENDER,NAME,BIRTHPLACE.
##"DOG " AND "CAT" CAN BE CONSIDERED  AS TYPE OF ANIMAL  HAVING PROPERTIES AGE,GENDER ,NAME,BIRTHPLACE.

#include <stdio.h>
int main(){
int n;
scanf("%d",&n);
struct animal
{
    int age;
    char gender;
    char *name;
    char *birthplace;
};//dog,cat;
struct animal dog,cat;//dog and cat are structure variable
dog.age=1;
dog.gender='F';
dog.name="kitty";
dog.birthplace="colarado";

cat.age=1;
cat.gender='M';
cat.name="kiy";
cat.birthplace="colado";
printf("%s",cat.name);
printf("%c",cat.gender);

}


#EASIER METHOD
#include <stdio.h>
int main(){
int n;
scanf("%d",&n);
struct animal
{
    int age;
    char gender;
    char *name;
    char *birthplace;
};

struct animal dog={3,'M',"kiyy","kiok"} ;
struct animal cat={3,'M',"ki","ok"} ;
printf("%s",cat.name);
printf("%c",cat.gender);


}


##ARRAY OF STRUCTURE VARIABLE

#include <stdio.h>
int main(){
int n;
scanf("%d",&n);
struct animal
{
    int age;
    char gender;
    char *name;
    char *birthplace;
    char *type;
};
struct animal a[3];
a[0].age=3;
a[0].name="Ace";
a[0].gender="M";
a[0].birthplace="fjlkd";
a[0].type="dog";

a[1].age=2;
a[1].name="ce";
a[1].gender='F';
a[1].birthplace="lkd";
a[1].type="cat";

a[2].age=5;
a[2].name="e";
a[2].gender='F';
a[2].birthplace="lkd";
a[2].type="tiger";
for (int i =0;i<2;i++)
{
    printf("\nAnimal is %s",a[i].type);
    printf("\nGENDER Is %c",a[i].gender);
    printf("\n");
}

}





##FILE IN C 


#include <stdio.h>
int main(){
//C:\Users\home\Documents\c\c program\fj
FILE *fp;//(fp is the pointer of type file this pointer is used to open read and close opeartion on the file)
fp=fopen("C:/Users/home/Documents/c/c program/fj/READ.txt","r");// (fp is now pointing to read.txt)   //this take two parameter 1st is the location 2nd is the mode of operation
char ch=fgetc(fp);
printf("%c",ch);
 ch=fgetc(fp);
printf("%c",ch);

return 0;

}

##using while loop
#include <stdio.h>
int main(){
//C:\Users\home\Documents\c\c program\fj
FILE *fp;//(fp is the pointer of type file this pointer is used to open read and close opeartion on the file)
fp=fopen("C:/Users/home/Documents/c/c program/fj/READ.txt","r");// (fp is now pointing to read.txt)   //this take two parameter 1st is the location 2nd is the mode of operation
while (1)
{


char ch=fgetc(fp);

if (ch==EOF)
{
    break;
}
printf("%c",ch);
}

return 0;

}



##WRITE TEXT INTO A FILE AND SAVE IT


#include <stdio.h>
int main(){
//C:\Users\home\Documents\c\c program\fj
FILE *fp;//(fp is the pointer of type file this pointer is used to open read and close opeartion on the file)
fp=fopen("C:/Users/home/Documents/c/c program/fj/WRITE.txt","w");// (fp is now pointing to read.txt)   //this take two parameter 1st is the location 2nd is the mode of operation
fprintf(fp,"%s","this is my first file");//file pointer ,format specifier ,string that needs to be entered
fclose(fp);
return 0;

}











           
