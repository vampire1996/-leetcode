# 7. Reverse Integer
<img src="https://github.com/vampire1996/LeetCode/blob/master/Problems/1-100/7.ReverseInteger/problem.png "/>

## c solution
```c
int reverse(int x) {
    int revertedX=0;
    int a;
    if(x!=0)
    {
        while(x%10==0) x=x/10;
    } 
      while(x!=0)
        {
            revertedX= revertedX*10+x%10;
          if(x<10)
              a=x;
            x=x/10;
        } 
   if(revertedX%10!=a) return 0;//检测revertedX是否溢出
    return revertedX;
}
```
