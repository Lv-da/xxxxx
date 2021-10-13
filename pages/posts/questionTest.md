---
title: 尝试一下出题
date: 2021/10/13
description: 第一次试试看看行不行.
tag: firstTry
author: 驴哒
---

# 第一次在大场面整活

第一次在oj上~~整活~~出题
```
#include <stdio.h>

int main()
{
    int i,n=0,f,t,w,m,p=2,x;
    scanf("%d",&x);
    for(i=0;i<x;i++){
        scanf("%d %d %d",&t,&f,&w);
        if(w==1){
            p++;
        }
        if(f==1){
            p++;
        }
        if(p>0){
        n = n + p*t;
        }
        if(t>=10){
            p--;
        }else if(t<=2){
            p=p+2;
        }
    }
    printf("%d",n);

    return 0;
}
```

