#include <stdio.h>
#include <math.h>

int main(){

    int A, B, C;
    float D;
    float R1, R2;

    printf("Coloque o valor de A: ");
    scanf("%d", &A);

    printf("Coloque o valor de B: ");
    scanf("%d", &B);

    printf("Coloque o valor de C: ");
    scanf("%d", &C);

    D = B * B - 4 * A * C;

    if(D < 0){
        printf("Nao existem raizes reais.\n");
    }else{

        R1 = (-B + sqrt(D)) / (2 * A);
        R2 = (-B - sqrt(D)) / (2 * A);

        printf("RESULTADO R1: %.2f\n", R1);
        printf("RESULTADO R2: %.2f\n", R2);
    }

    return 0;
}
