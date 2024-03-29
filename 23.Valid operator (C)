#include <stdio.h>
#include <stdbool.h>
#include <ctype.h>

// Function to check if a character is a valid operator
bool isOperator(char c) {
    return (c == '+' || c == '-' || c == '*' || c == '/');
}

// Function to perform lexical analysis
void lexicalAnalyzer(const char *input) {
    int i = 0;
    printf("Operators found:\n");
    while (input[i] != '\0') {
        if (isOperator(input[i])) {
            printf("'%c' is a valid operator\n", input[i]);
        }
        i++;
    }
}

int main() {
    char input[100];
    
    printf("Enter an expression: ");
    fgets(input, sizeof(input), stdin); // Read input from user
    
    // Call the lexical analyzer function
    lexicalAnalyzer(input);
    
    return 0;
}
