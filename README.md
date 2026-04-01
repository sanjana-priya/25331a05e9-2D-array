#include<stdio.h>
int main() {
    int r, c, i, j;
    int m1[50][50], m2[50][50], sum[50][50];

    printf("Enter rows and columns (max 50): ");
    scanf("%d %d", &r, &c);

    
    printf("Enter elements of 1st matrix:\n");
    for (i = 0; i < r; ++i)
        for (j = 0; j < c; ++j)
            scanf("%d", &m1[i][j]);

    
    printf("Enter elements of 2nd matrix:\n");
    for (i = 0; i < r; ++i)
        for (j = 0; j < c; ++j)
            scanf("%d", &m2[i][j]);

    for (i = 0; i < r; ++i)
        for (j = 0; j < c; ++j)
            sum[i][j] = m1[i][j] + m2[i][j];

    
    printf("\nSum:\n");
    for (i = 0; i < r; ++i) {
        for (j = 0; j < c; ++j)
            printf("%d ", sum[i][j]);
        printf("\n");
    }
    return 0;
}
