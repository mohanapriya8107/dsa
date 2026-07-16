  // without sorting find the firstmax anf second max
#include <stdio.h>
int main(){
int n,max,smax=-1,curr;
scanf("%d%d",&n,&max);
for(int i=2;i<=n;i++){
    scanf("%d",&curr);
    if(curr>max){      
        smax=max;        
        max=curr;   
    }else if(curr>smax){
        smax=curr;
    }
}
printf("%d %d",max,smax);
}

