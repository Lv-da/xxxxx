---
title: cHomework2
date: 2021/10/18
description: cHomework2.
tag: Homework
author: 驴哒
---

# c语言作业2answer

猜猜有哪些地方容易错？

~~反正我是不记得了~~

#### 让我康康有多少人来看（
![](https://count.getloli.com/get/@Lv-da?theme=rule34)

#### 加了个聊天室，可以来氵或者问问题，看看有没有其他人回答你（
直接点进去就行
[![SVG Charts](https://chat.getloli.com/room/@Lv-da/svg?width=750&height=360&limit=20&theme=light&fontSize=13&title=Lv-da@github.com:%20%7E)](https://chat.getloli.com/room/@Lv-da?title=Lv-da)

## Problem A.
```
#include <stdio.h>
int main()
{
    int a[101];
    int n,i,sum = 0;
    int x,j;
    scanf("%d",&x);
    for(j=0;j<x;j++)
    {
        scanf("%d",&n);
        for(i=0;i<n;i++){
            scanf("%d",&a[i]);
        }
        sum = 0;
        for(i=0;i<n;i++){
            sum = sum + a[i];
        }
        printf("%d\n",sum);
    }

    return 0;
}
```

## Problem B.
```
#include <stdio.h>
#include <math.h>

int duan(int a,int b)
{
    return a<b?a:b;
}

int main()
{
    int h,w,a,b,duande;
    while(scanf("%d %d %d %d",&h,&w,&a,&b)!=EOF){
        duande = duan(a,b);
        if(sqrt(h*h+w*w)>=duande){
            printf("Just do it.\n");
        }else{
            printf("We have a problem.\n");
        }
    }
    
    return 0;
}
```

## Problem C.
```
#include <stdio.h>

int main()
{
    double e=1,n=1,m,i,j,k;
    int count=1;
    for(i=1;n>=0.00001;i++){
        j=1;
        for(k=1;k<=i;k++){
            j = j * k;
        }
        n = 1.0/j;
        e = e + n;
        count++;
    }
    printf("%lf %d",e,count);

    return 0;
}
```

## Problem D.
```
#include <stdio.h>
#include <math.h>

int main()
{
    unsigned long long int num=1,sum=0;
    double v;
    for(int i=0;i<64;i++){
        sum = sum + num;
        num = 2*num;
    }
    v = sum/142000000.0;
    printf("%llu\n%lf",sum,v);

    return 0;
}
```
注意数据范围

## Problem E.
```
#include <stdio.h>

int main()
{
    int a[11]={0},i,b;
    for(i=1;i<10;i++){
        scanf("%d",&b);
        a[b]=1;
    }
    for(i=1;i<=10;i++){
        if(a[i]==0){
            printf("The missing integer is:%d",i);
        }
    }

    return 0;
}
```

## Problem F.
```
#include <stdio.h>

int main()
{
    int n,m,i,j;
    int sum = 0;
    scanf("%d",&n);
    for(m=1;sum<n;m++){
        j=1;
        for(i=1;i<=m;i++){
            j = j * i;
        }
        sum = sum + j;
    }
    printf("%d",m-2);

    return 0;
}
```

## Problem G.
```
#include<stdio.h>
#include<math.h>

int main(){
	int W,S,X,Y;
	int mould[10000][100];
	int max[100];
	int cur;
	scanf("%d%d",&W,&S);
	scanf("%d%d",&X,&Y);
	for(int i = 0;i < W;i++){
		for(int j = 0;j < X;j++){
			scanf("%d",&mould[i][j]);
		}
	}
	
	
	for(int i = 0;i < S;i++){
		for(int j = 0;j < X;j++){
			scanf("%d",&cur);
			if(cur > max[j]){
				max[j] = cur;
			} 
		}
	}
	

	for(int i = 0;i < W;i++){
		for(int j = 0;j < X;j++){
			if(Y-mould[i][j] < max[j]){
				mould[i][j] = Y-max[j];
			}
			if(j == 0){
				printf("%d",mould[i][j]);
			}else{
				printf(" %d",mould[i][j]);
			}
		}
		printf("\n");
	}
	
	return 0;
}
```

### Finish.

![微信图片_20211018125947.jpg](https://i.loli.net/2021/10/18/XiMICASaUzoFOp6.jpg)

