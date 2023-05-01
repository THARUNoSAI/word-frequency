#include <stdio.h>
#include <string.h>

int main() {
    char str[100];
    int i, j, len, freq = 0, repeated = 0;
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);
    len = strlen(str) - 1; 
    printf("Length of the string is: %d\n", len);
    for (i = 0; i < len; i++) {
        int flag = 0;
        for (j = i + 1; j < len; j++) {
            if (str[i] == str[j]) {
                flag = 1;
                break;
            }
        }
        if (!flag) {
            freq++;
        }
    }
    printf("Word frequency is: %d\n", freq);
    for (i = 0; i < len; i++) {
        for (j = i + 1; j < len; j++) {
            if (str[i] == str[j]) {
                printf("First repeated character is: %c\n", str[i]);
                repeated = 1;
                break;
            }
        }
        if (repeated) {
            break;
        }
    }
    if (!repeated) {
        printf("No repeated characters found in the string.\n");
    }
    for (i = 0; i < len; i++) {
        int flag = 0;
        for (j = 0; j < len; j++) {
            if (i != j && str[i] == str[j]) {
                flag = 1;
                break;
            }
        }
        if (!flag) {
            printf("First non-repeated character is: %c\n", str[i]);
            break;
        }
    }
    return 0;
}
