#include <stdio.h>
#include <conio.h>

void shiftCipher(char* text, int shift) 
{
    int i = 0;
    while (text[i] != '\0') 
    {
        char ch = text[i];
        // Encrypt for uppercase letters
        if (ch >= 'A' && ch <= 'Z') 
        {
            text[i] = ((ch - 'A' + shift) % 26) + 'A';
        }
        // Encrypt for lowercase letters
        else if (ch >= 'a' && ch <= 'z') 
        {
            text[i] = ((ch - 'a' + shift) % 26) + 'a';
        }
        i++;
    }
}

int main() 
{
    char text[] = "Kush";
    int shift;
    clrscr();
    printf("Enter any Shift Value:");
    scanf("%d",&shift);
    printf("Normal text: %s\n", text);
    shiftCipher(text, shift);
    printf("Encrypted text: %s\n", text);
    getch();
    return 0;
}
