# cs50
Cs-50-course



#include <stdio.h>
#include <cs50.h>

int main(void)
{
   int height;

    // ask user to spicify hight
    while (height < 0 || height > 23)
    {
        printf("Please specify the height of the pyramid: ");
        height = get_int("height is:");
    }
    

    // for loops specifying number of spaces and hashes per line
    for (int i = 0; i < height; i++)
    {
        for (int j = height - i; j > 1; j--)
        {
            printf(" ");
        }
        for (int hashes = 0; hashes < i + 2; hashes++)
        {
            printf("#");
        }
        printf("\n");
    }
}
