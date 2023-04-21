# Bubble-sort
#include<stdio.h>
           int main(){
    int t;
    scanf("%d",&t);
    while(t>0){
        int n,i,j;
        scanf("%d",&n);
        int arr[n];
        for(i=0;i<n;i++){
            scanf("%d",&arr[i]);
        }
        for(i=0;i<n;i++){
            for(j=i+1;j<n;j++){
                if(arr[i]>arr[j]){
                    int temp=arr[i];
                    arr[i]=arr[j];
                    arr[j]=temp; }
        }
        int a,b;
        scanf("%d%d",&a,&b);
        int sum=0;
        for(i=a;i<b-1;i++){
            sum+=arr[i];
        }
        printf("\n%d",sum);
        t--;
    }
       
return 0;
}
