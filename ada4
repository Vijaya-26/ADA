#include<stdio.h>
#include<time.h>
#include<stdlib.h>

void insertionsort(int n, int a[])
{
    int i, key, j;
    for (i = 1; i < n; i++)
    {
        key = a[i];
        j = i - 1;
        while (j >= 0 && a[j] > key)
        {
            a[j + 1] = a[j];
            j = j - 1;
        }
        a[j + 1] = key;
    }
}

void main()
{
    int a[15000] , n , i , j , ch , temp;
    clock_t start , end;

    while(1)
    {
        printf("\n1:Insertion \n2:Display time taken \n3. Exit");
        printf("\n Enter your choice:");
        scanf("%d", &ch);
        switch(ch)
        {
            case 1: printf("\nEnter the number of elements: ");
                    scanf("%d", &n);
                    printf("\nEnter elements: ");
                    for(i = 0 ; i<n ; i++)
                    {
                        scanf("%d", &a[i]);
                    }
                    start = clock();
                    insertionsort(n , a);
                    end = clock();
                    printf("\nSorted array is : ");
                    for(i = 0 ; i< n ; i++)
                    printf("%d\t", a[i]);
                    printf("\n Time taken to sort %d number is %f Secs" , n , (((double)(end-start))/CLOCKS_PER_SEC));

                break;

            case 2 : n = 500;
                        while(n <= 14500)
                        {
                            for(i = 0 ; i <n ; i++)
                            {
                                a[i] = n - i;
                            }
                            start  = clock();
                            insertionsort(n , a);
                            for(j = 0 ; j < 500000; j++)
                            {
                                temp = 38/600;
                            }
                            end = clock();
                            printf("\n Time taken to sort %d number is %f Secs" , n , (((double)(end-start))/CLOCKS_PER_SEC));
                            n = n + 1000;

                        }

                        break;

            case 3: exit(0);

        }
        getchar();

    }

}
