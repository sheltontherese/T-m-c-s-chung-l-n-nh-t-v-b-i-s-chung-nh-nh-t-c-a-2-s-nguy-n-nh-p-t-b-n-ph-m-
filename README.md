# T-m-c-s-chung-l-n-nh-t-v-b-i-s-chung-nh-nh-t-c-a-2-s-nguy-n-nh-p-t-b-n-ph-m-
Tìm ước số chung lớn nhất và bội số chung nhỏ nhất của 2 số nguyên nhập từ bàn phím  
#include<stdio.h>
#include<conio.h>
#include<conio.h>
main()
{            
    int x,y,a,b;
    do
    {
        printf("Nhap a,b = ");
        scanf("%d%d",&a,&b);
    }
    while(a<=0 || b<=0);
    x=a;
    y=b;
    while(a!=b)
    {
        if(a>b)
        {
            a-=b;
        }
        else
        {
            b-=a;    
        }
    }
    printf("Uoc chung lon nhat la %d",a);
    printf("\nBoi chung nho nhat la %d",(x*y)/a);
    getch();
}
