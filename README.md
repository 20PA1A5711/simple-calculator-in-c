# simple-calculator-in-c
#include <stdio.h> 

int main()  
{  
    char opt;  
    int n1, n2;   
    float res;  
    printf (" Choose an operator(+, -, *, /) to perform the operation in C Calculator \n ");  
    scanf ("%c", &opt); 
    printf (" \n Enter the first number: ");  
    scanf(" %d", &n1);
    printf (" Enter the second number: ");  
    scanf (" %d", &n2); 
      switch(opt)  
    {  
        case '+':  
            res = n1 + n2;   
            printf (" Addition of %d and %d is: %.2f", n1, n2, res);  
            break;  
          
        case '-':  
            res = n1 - n2;  
            printf (" Subtraction of %d and %d is: %.2f", n1, n2, res);  
            break;  
              
        case '*':  
            res = n1 * n2; 
            printf (" Multiplication of %d and %d is: %.2f", n1, n2, res);  
            break;            
          
        case '/':  
            if (n2 == 0)    
            {  
                printf (" \n Divisor cannot be zero. Please enter another value ");  
                scanf ("%d", &n2);        
                }  
            res = n1 / n2;  
            printf (" Division of %d and %d is: %.2f", n1, n2, res);  
            break; 
    
        default:    
            printf (" Something is wrong!! Please check the options ");               
    }  
    return 0;  
}  



output:
Choose an operator(+, -, *, /) to perform the operation in C Calculator 
 *
 Enter the first number: 2
 Enter the second number: 3
 Multiplication of 2 and 3 is: 6.00
