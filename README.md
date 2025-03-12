# c-19
string reverse
#include<stdio.h>
#include<string.h>
#include<stdlib.h>
int main()
{
    char str[50],temp;
    int i,length;
    printf("enter a name:\n");
    scanf("%s",str);
    length=strlen(str);
    for(i=0;i<length/2;i++){
        temp=str[i];
        str[i]= str[length-i-1];
        str[length-i-1]=temp;
    }
    printf("Reversed string is %s\n",str);
    return 0;
}
