# 657. Robot Return to Origin
<img src="https://github.com/vampire1996/LeetCode/blob/master/Problems/601-700/657.RobotReturnToOrigin/problem.png"/>
<img src="https://github.com/vampire1996/LeetCode/blob/master/Problems/601-700/657.RobotReturnToOrigin/example.png"/>

## c solution
```c
bool judgeCircle(char* moves) {
    int cntU=0,cntD=0,cntL=0,cntR=0;
    int len=strlen(moves);
    for(int i=0;i<len;i++)
    {
        switch(moves[i])
        {
         case 'U':cntU++;continue;
         case 'D':cntD++;continue;
         case 'L':cntL++;continue;
         case 'R':cntR++;continue; 
         default: return false;       
        }
    }
    if(cntU==cntD&&cntL==cntR) {return true;}
    else     {return false;} 
}
```
