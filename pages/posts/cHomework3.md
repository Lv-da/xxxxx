---
title: cHomewor3
date: 2021/10/25
description: cHomework3.
tag: Homework
author: 驴哒
---

# c语言作业1answer

~~开摆了兄弟们~~

```
#include <stdio.h>

int main()
{
	int a;
	scanf("%d",&a);
	if(a==1){
		printf("18000");
	}else{
		printf("0");
	}
	return 0;
}
```
```
#include<stdio.h>
int main()
{
    int a,b,c;
    scanf("%d %d %d",&a,&b,&c);
    printf("%f",(float)((float)(a+b+c)/3.0));
}
```
```
#include<stdio.h>
#include<math.h>
int main()
{
    int a;
    scanf("%d",&a); 
    double ans=(float)a*3.141592653/180; 
    printf("%.6f\n%.6f\n",sin(ans),cos(ans)); 
    return 0; 
}
```
```
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    switch (a)
    {
    case 1:
        printf("2");
        break;
    case 2:
        printf("3");
        break;
    case 3:
        printf("1");
        break;
    }

    return 0;
}
```
```
#include<stdio.h>

int main()
{ 
    int n,m;
    scanf("%d",&n);
    int sum1=5,sum2=0;
    int i; 
    for(i=1;i<=n;i++)
    {
        scanf("%d",&m); 
        if(m>=10)
        {
            sum1=sum1+1;
        }
        if(m>=5)
        {
            sum2=sum2+1;    
        }   
    }   
    
    if(sum1>sum2){
        printf("%d",sum2);
    } 
    else
    {
        printf("%d",sum1);
    } 

    return 0;
} 
```
```
#include<stdio.h>
#include<math.h>
int solve(int x){
    if(x==11) return 3;
    if(x==15) return 0;
    if(x==2) return 2;
    for(int i = 2;i<sqrt(x)+0.5;++i){
        if(x%i==0) return 1;
    }
    return 2;
}
int main(){
    int r,n,q;
    int ans1,ans2;
    scanf("%d%d",&r,&n);
    if(n%2==0 && r%2==1)
        q = r/2 + 1;
    else
        q = r/2;
    ans1 = 0; ans2 = (r-q)*2;
    for(int i = 0;i<q;++i){
        int L;
        scanf("%d",&L);
        ans1+=solve(L);
    }
    if(ans1==ans2)     printf("equal.");
    else if(ans1>ans2) printf("lwh wins.");
    else               printf("lzh wins.");
}
```
```
#include<stdio.h>
#include <string.h>
int main(){
    int matrix[30][30],temp[30][30];
    int n,m;
    scanf("%d%d",&n,&m);
    for(int i = 1;i<=n;++i)
        for(int j = 1;j<=n;++j)
            scanf("%d",&matrix[i][j]);
    for(int k = 1;k<=m;++k){
        int x;
        scanf("%d",&x);
        memcpy(temp,matrix,sizeof(matrix));
        for(int i = 1;i<=n;++i){
            for(int j = 1;j<=n;++j){
                switch(x){
                    case 1:
                        matrix[j][n-i+1] = temp[i][j];
                        break;
                    case 2:
                        matrix[n-j+1][i] = temp[i][j];
                        break;
                    case 3:
                        matrix[n-i+1][n-j+1] = temp[i][j];
                        break;
                }
            }
        }
        for(int i = 1;i<=n;++i){
            for(int j = 1;j<=n;++j){
                printf("%d",matrix[i][j]);
                if(j!=n) printf(" ");
            }
            printf("\n");
        }
        printf("\n");
    }
    return 0;
}
```
