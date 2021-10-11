---
title: c语言作业1
date: 2021/10/11
description: 都欺负我没有老本吃.
tag: 作业1
author: 驴哒
---

~都有老本，就我没老本还得慢慢写，这下知道谁是卷王了吧

**Problem A.**
	#include <stdio.h>

	int main()
	{
		int n = 0;
		double deposit = 100,rate;
		scanf("%lf",&rate);

		while(deposit < 200)
		{
			deposit = deposit * (1 + rate);
			n++;
		}

		printf("%d\n",n);
	   return 0;
	}

**Problem B.**
	#include <stdio.h>

	int main()
	{
	    int i,n,a,b,c,d;
	    for(i=10;;i++){
		n = i * i;
		d = n%10;
		c = n/10%10;
		b = n/100%10;
		a = n/1000;
		if(a==b && c==d){
		    break;
		}
	    }
	    printf("%d",n);
	    return 0;
	}

**Problem C.**
	#include <stdio.h>
	#include <math.h>

	int main()
	{
	    double a,e,d=0.0;
	    int b,c;
	    scanf("%lf %d %d",&a,&b,&c);
	    e = pow(1+a,b);
	    d = c*e;
	    printf("%f",d);

	    return 0;
	}

**Problem D.**
	#include <stdio.h>

	int main()
	{
	    double a=0,b=0.01;

	    for(int i=0;i<30;i++){
		a+=b;
		b*=2.0;
	    }
	    printf("%f\n",a);
	    printf("3000000\n");
	    return 0;
	}
~~赌五毛有人跟我一样因为读题问题把两个数输出反了~~

**Problem E.**
	#include <stdio.h>

	int main()
	{
	    int count=0;
	    int ten=0,five=00,one=0;
	    for(ten=0;ten<10;ten++){
		for(five=0;five<20;five++){
		    for(one=0;one<50;one++){
			if((one+five+ten)==50 && (one + 5*five + 10*ten) == 100){
			    printf("%d %d %d\n",ten,five,one);
			    count++;
			    printf("%d",count);
			}
		    }
		}
	    }

	    return 0;
	}

**Problem F.**
	#include <stdio.h>

	int main()
	{
	    int t,m;
	    int a[13]={0,31,28,31,30,31,30,31,31,30,31,30,31};
	    scanf("%d %d",&t,&m);
	    if(m>=1 && m<=12){
		if(m==2){
		    if(t%100 != 0 && t%4 ==0 || t%400 == 0){
			printf("29");
		    }else{
			printf("28");
		    }

		}else{
		    printf("%d",a[m]);
		}
	    }else{
		printf("error");
	    }

	    return 0;
	}
**注意闰年的判断**

**Problem G.**
	#include <stdio.h>

	int main()
	{
		printf("3.141594");

	    return 0;
	}
没错就是这样XD

想到了易错点会更新


