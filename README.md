# palindrome
 

#include <stdio.h>
#include <string.h>

int pan(char str[]){
    int i,n;
    char c;
    n=strlen(str);
    for(i=0;i<n/2;i++){
        if(str[i]!=str[n-i-1]){
            return 0;
        }}
      return 1;
      
}

int main(){
    char str[200];
    printf("Enter a Name: ");
    scanf("%[^\n]s",str);

   if (pan(str)) {
        printf("It is a Palindrome.\n");}
    else {
        printf("NOT a Palindrome.\n");}
        return 0;
}
