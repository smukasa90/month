#include <stdio.h>
int main(){
	int days, start, i, x, j = 0;
	printf("please enter the number of days in the month: ");
	scanf("%d", &days);
	printf("\nplease enter the starting day (sun = 1 and sat = 7): ");
	scanf("%d", &start);
	printf("\n");
	printf("su mo tu we th fr sa");
	printf("\n");
	for(x = 1; x < start; x++){
		printf("   ");
		j += 1;
	}
	for(i = 1; i <= days; i++){
		j += 1;
		if(i < 10){
			printf(" %d ", i);
			if((j%7) == 0){
				printf("\n");
			}
		}
		else{
			printf("%d ", i);
			if((j%7) == 0){
				printf("\n");
			}
		}
	}	
}
