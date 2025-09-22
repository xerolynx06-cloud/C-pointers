//# C-pointers
//Hi im Xero this is my 1st repository in GitHub this is my c basic level pointer program i love c program but im a beginner
#include<stdio.h>
void typeHour(int *p_hours); //Function Prototype
int main(){
   int hours = 6; //Im Declaring a variable
   int *pHours = &hours; // here i used pointer basically pointer just allows us to nagvigate where our value is stored
   printf("Time Right Now:%dam\n",hours);
   printf("Memory Pointer:%p\n",(*void)pHours);
   typeHour(pHours);
   printf("Time After a Hour:%d\n",hours);
   return 0;
}
void typeHour(int *p_hours){
  (*p_Hours)++;
}
