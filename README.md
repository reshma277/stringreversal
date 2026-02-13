# stringreversal
Reversing a string without using a built in function 
#include <stdio.h>
#include <string.h>

int main() {
    char arr[] = "coading";

    char *a = &arr[1];
    char *b = &arr[6];
    char temp;

    while (a < b) {
        temp = *a;
        *a = *b;
        *b = temp;

        a++;
        b--;
    }

    printf("Reversed string: %s\n", arr);

    return 0;
}