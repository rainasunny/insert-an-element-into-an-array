# insert-an-element-into-an-array
#include <stdio.h>
int main() {
     int arr[70],pos,i,n,val;
    printf("Enter the size of array, max 70 \n");
    scanf("%d",&n);
    printf("Enter %d elements one by one\n",n);
    for(i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
        }
        printf("Enter the location to insert the element\n");
        scanf("%d",&pos);
        printf("Enter the value to be inserted\n");
        scanf("%d",&val);
        for(i=n-1;i>=pos;i--)
        {
            arr[i+1]=arr[i];
            }
            arr[pos]=val;
            printf("Updated array\n");
            for(i=0;i<=n;i++)
            {
                printf("%d\n",arr[i]);
}
        
    
    return 0;
}
