# CS-EASY-01 Hello world!--Answer Sheet

### 第一个程序

1. 高级计算机语言更接近人类语言逻辑，入门容易，可读性强，但更难以接触计算机运行的本质。低级计算机语言更接近计算机的二进制语言，更接近计算机的运行本质，可入门更难，没有那么人性化。我更喜欢高级计算机语言。

2. 解读hello.c

   ```c
   #include <stdio.h> /*对编译器发出指示，表明该程序包含Standard I/O头文件。据此可启动下文的各个函数。*/
   
   int main() { //主函数，表明程序的开始。int定义main的返回类型为整形。
       printf("Hello, world!"); //printf函数意味着输出，引号中的是输出的内容。
       return 0; //向main函数返回值0，表明程序结束，
   } 
   ```

3. 行2

4. int类型指整形元素，即整数。整数中0是最简单，中性，对程性最好的数字，用int声明main，即可返回0，是最简单，最自然表明程序成功运行的方式。

5.  

   ![hello world.c - C - Visual Studio Code 2024_9_25 21_40_03](C:\Users\Cai\Videos\Captures\hello world.c - C - Visual Studio Code 2024_9_25 21_40_03.png)

## 基础语法运用

修改后的代码: 

```c
#include <stdio.h>

int main() 
{
    int code;

start:
    printf("Show me your code,please.\n");
    scanf("%d", &code);
    if(code >= 100000 && code <= 999999)
    {
        printf("I am super hacker!\n");
    }
    else 
    {
        printf("Fake code!\n"); 
        goto start;
    }
    return 0;
}
```



## 课后题

```c
#include <stdio.h> 

int main() 
{
    int m,n;
start:
    printf("Please give two integers.\nm="); 
    scanf("%d", &m); 
    printf("n=");
    scanf("%d", &n); 
    if (m <= 0 || m >= 2147483648 || n <= 0 || n >= 2147483648)
    {
        goto start;
    }
    while (m != 0 && n != 0)
    {
     if (m >= n)
     {
        m = m-n;
     }
     else
     {
        n = n-m;
     }
    }
    if (m = 0)
    {
        printf("The greatest common divisor:%d", n);
    }
    else if (n = 0)
    {
        printf("The greatest common divisor:%d", m);
    }
}
```

