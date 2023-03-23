# 4주차 C언어 실습
``` c
#include <stdio.h>

int main(void)

{
    int money, change;
    int price, c5000, c1000, c500, c100, c10;
    
    printf("물건 값을 입력하시오: ");
    scanf("%d", &price); 

    printf("투입한 금액을 입력하시오: ");
    scanf("%d", &money); 

    change = money - price; 

    c1000 = change / 1000; 
    change = change % 1000; 

    c500 = change / 500; 
    change = change % 500; 

    c100 = change / 100; 
    change = change % 100; 

    c10 = change / 10; 
    change = change % 10; 


    printf("\n천원권: %d장\n", c1000);
    printf("오백원 동전: %d개\n", c500);
    printf("백원 동전: %d개\n", c100);
    printf("십원 동전: %d개\n", c10);

    return 0;

}

```

``` c
#include <stdio.h>

int main(viod)

{
    
    int x=10, y=10;

    printf("x=%d\n", x);
    printf("++x의 값=%d\n", ++x);
    printf("x=%d\n\n", x);

    printf("y=%d\n", y);
    printf("++y의 값=%d\n", ++y);
    printf("y=%d\n\n", y);

    return 0;

}

```

``` c
#include <stdio.h>

int main()

{
    double x, y, result;

    printf("두개의 실수를 입력하시오: ");
    scanf("%lf %lf", &x, &y);
    
    result = x + y;
    printf("%lf + %lf = %lf\n", x, y, result);
    
    result = x - y; 
    printf("%lf - %lf = %lf\n", x, y, result);
    
    result = x * y;
    printf("%lf + %lf = %lf\n", x, y, result);
    
    result = x / y; 
    printf("%lf / %lf = %lf\n", x, y, result);
    
    return 0;
}

```

```c

#include <stdio.h>

int main()

 {

    int n1, n2;
    scanf("%d %d", &n1, &n2);

    int n3 = n1 * (n2 % 10);
    int n4 = n1 * (n2 / 10 % 10);
    int n5 = n1 * (n2 / 100);

    printf("%d\n", n3);
    printf("%d\n", n4);
    printf("%d\n", n5);
    printf("%d\n", n5*100 + n4*10 + n3);

    return 0;

 }
 
 ```
