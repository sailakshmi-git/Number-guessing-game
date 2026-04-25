# Number-guessing-game
Write a C program for a number guessing game where the loop continues for wrong guesses, breaks on a correct guess, and exits the program using return if the user enters -1.

Program:

```
#include <stdio.h>

int main() {
    int secret = 7;
    int guess;

    while(1) {
        printf("Enter your guess (-1 to exit): ");
        scanf("%d", &guess);

        if(guess == -1) {
            printf("Exiting game...\n");
            return 0;
        }

        if(guess == secret) {
            printf("Correct guess!\n");
            break;
        }

        printf("Wrong guess, try again.\n");
    }

    return 0;
}
```

Output:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a349cd8b-d006-4962-99f3-deee12b557fc" />
