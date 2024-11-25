#include <stdio.h>

void print_binary(int num) {
    int i;
    for (i = 31; i >= 0; --i) {
        (num & (1 << i)) ? printf("1") : printf("0");
    }
}

int main() {
    int num;

    printf("Enter an integer: ");
    scanf("%d", &num);

    printf("Binary representation: ");
    print_binary(num);
    printf("\n");

    printf("Octal representation: %o\n", num);
    printf("Hexadecimal representation: %x\n", num);

    return 0;
}
