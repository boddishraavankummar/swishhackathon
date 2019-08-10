#include<stdio.h>
int main(){
	int x,p;
	int money;
	int percent,per;
	scanf("%d %d",&x,&p);
	money = x;
	percent = x * p;
	while(percent != 0){
		per = p * x;
		percent = per / 100;
		if(percent == 0){
		    break;
		}
		x = x - percent;
		money = money + x;
	}
	printf("%d",money);
	return 0;
}
