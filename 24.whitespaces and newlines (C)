#include <stdio.h>
#include <ctype.h>

// Function to perform lexical analysis
void lexicalAnalyzer(const char *input, int *whitespaceCount, int *newlineCount) {
    int i = 0;
    while (input[i] != '\0') {
        if (isspace(input[i])) {
            if (input[i] == '\n') {
                (*newlineCount)++;
            } else {
                (*whitespaceCount)++;
            }
        }
        i++;
    }
}

int main() {
    char input[1000];
    int whitespaceCount = 0, newlineCount = 0;
    
    printf("Enter some text (press Ctrl+D to finish):\n");
    
    // Read input from user until EOF
    while (fgets(input, sizeof(input), stdin) != NULL) {
        // Call the lexical analyzer function for each line of input
        lexicalAnalyzer(input, &whitespaceCount, &newlineCount);
    }
    
    printf("Number of whitespace characters: %d\n", whitespaceCount);
    printf("Number of newline characters: %d\n", newlineCount);
    
    return 0;
}
