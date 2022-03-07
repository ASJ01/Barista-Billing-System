#include<stdio.h>
#include<conio.h>
#include<string.h>
void main(){
    int q[10],i,j,x;                                                  //variables
    float r[10],p[10],t=0;
    char n[10][25];
    printf("Welcome to BARISTA");                        //title
    for(i=1;i<=10;i++)
    {
        gets(n[i]);                                                
        printf("Enter Product Name=");                                      //product details
        gets(n[i]);
        printf("Enter The Quantity=");                 
        scanf("%d",&q[i]);
        printf("Enter Price=");
        scanf("%f",&r[i]);
        p[i]=r[i]*q[i];
        j=i;
        t=t+p[i];
        printf("\nEnter any key to Add more\n Enter 0 to Make the Bill:");
        scanf("%d",&x);
        if(x==0)
        { break;}
        
}
printf("\n\tBARISTA");
printf("\n\t===============================================================");                 //print bill
printf("\n \t Product \t\t Qty \t rate \t price");
for(i=1;i<=j;i++)
{
    printf("\n\t %s \t\t %d \t %0.2f \t %0.2f",n[i],q[i],r[i],p[i]);
    
}
printf("\n\t\t Total=%0.2f",t);
printf("\n\t===============================================================");
printf("\n THANK YOU VISIT AGAIN");                                                                                      //ending
getch();
}
