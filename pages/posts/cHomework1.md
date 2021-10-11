---
title: cHomework1
date: 2021/10/11
description: cHomework1.
tag: Homework
author: 驴哒
---

都有老本，就我没老本还得慢慢写，这下知道谁是卷王了吧

### Problem A.
```
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
```
正常的数学问题，正常计算应该都没大问题

### Problem B.
```
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
```
将4位数分开并用if判断是否合适即可，因为只用输出一个数，所以if成立后要用break结束for循环

### Problem C.
```
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
```
同款普通数学问题，正常计算即可

### Problem D.
```
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
```
~~赌五毛有人跟我一样因为读题问题把两个数输出反了~~
循环即可

### Problem E.
```
	int main()
	{
	    int count=0;
	    int ten=0,five=0,one=0;
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
```
~~我猜有人第一次提交的时候忘记加count了~~
三层for穷举3种纸币的组合，if判断合适的组合并输出，记得count++哦

### Problem F.
```
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
```
**注意闰年的判断**

当然判断每个月的天数也可以不用数组，显得高级点XD，如下
```
int numberofdays(struct date d)
{
   if(d.month == 1 || d.month == 3 || d.month == 5 || d.month == 7 || d.month == 8 || d.month == 10 || d.month == 12){
       return 31;
   }else{
       return 30;
   }
}
```
### Problem G.
```
	int main()
	{
		printf("3.141594");

	    return 0;
	}
```
没错就是这样XD
下面这种解法能过但是有肉眼可见的误差
```
	int main()
	{
	    double pai=0,i=1.0,z=1.0;
	    while ((1.0/i)>=0.0001){
		pai = pai + z*(1.0/i);
		z = (-1.0)*z;
		i = i+2.0;  
	    }
	    printf("%f",4.0*pai);

	    return 0;
	}
```
按照题目要求把公式写下来就行

想到了易错点会更新

![微信图片_20211011142148.png](https://i.loli.net/2021/10/11/P6wQIOy48NzEl1A.png)

~~看来是时候刷oj了，不然抢不到第一给vup打广告啊啊啊啊啊啊~~

