#include <stdio.h>

int main() {
    int n, i;
    
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int numbers[n];

    // Input the numbers
    printf("Enter %d numbers:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &numbers[i]);
    }

    // Check for odd or even
    printf("\nResult:\n");
    for(i = 0; i < n; i++) {
        if(numbers[i] % 2 == 0)
            printf("%d is Even\n", numbers[i]);
        else
            printf("%d is Odd\n", numbers[i]);
    }

    return 0;
}
