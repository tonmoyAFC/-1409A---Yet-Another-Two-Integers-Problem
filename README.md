# -1409A---Yet-Another-Two-Integers-Problem Codeforces
#include <stdio.h>

int main() {
    int t,i;
    scanf("%d", &t);
    for  (i = 0; i<t; i++)
    {
        long long int a, b, c;
        scanf("%lld %lld", &a, &b);
        if(a==b)
        {
            printf("%lld\n",a-b);
            
        }
        else
        {
            if (a>b)
            {
                c = a-b;
                if (c%10 == 0)
                {
                    printf("%lld\n",c/10);
                }
                else if(c%10 != 0)
                {
                    printf("%lld\n",(c/10)+1);
                }
                
            }
            //
            
            else if(b>a){
                c = b-a;
                if(c%10 ==0)
                {
                    printf("%lld\n",c/10);
                }
                else if (c%10!= 0)
                {
                    printf("%lld\n",(c/10)+1);
                }
            }
        }
        
    }
    return 0;
    
    
  
}
