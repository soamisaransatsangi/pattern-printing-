#include <stdio.h>

int main() {
    int n = 5; // Number of rows

    for (int i = 0; i < n; i++) { // Loop for each row
        // Print leading spaces
        for (int j = 0; j < n - i - 1; j++) {
            printf(" ");
        }
        // Print the star at the beginning of the row
        printf("*");

        // Print spaces between the stars
        if (i > 0) {
            for (int j = 0; j < 2 * i - 1; j++) {
                printf(" ");
            }
            // Print the star at the end of the row
            printf("*");
        }

        // Move to the next line
        printf("\n");
    }

    return 0;
}
