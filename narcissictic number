// Louis Anton D. Saclot
// CSA-1
// Nov. 22, 2015
// This program will determine the number inputed if its a narcissistic or not.

#include <stdio.h>

int narnum(int num1);

int main() {
	
	int x;
	int num1=0;
	
	// Asks for input
	for(x=0;x<3;x++){
		
	printf("Please Enter a number: ");
	scanf("%d", &num1);

	// Displays if its a Narcissistic or not
	if(narnum(num1)==num1)
		printf("%d is a Narcissistic number.\n", num1);
	else
		printf("%d is not a Narcissistic number.\n", num1);
	}
}

int narnum(int num1) {
	
	int cnt=0, total=0, prod=1;
	int power,trynum,digit;
	
	trynum=num1; // trynum represents num1
	while(trynum>0) { // determines how many digits 
		trynum=trynum/10; 
		cnt++;
	}
	
	trynum=num1;
	while(trynum>0) {
		power=trynum%10;
		 
		while(digit<cnt) {
			prod=prod*power; 
			digit++;	
		}
		
		total=total+prod; 
		prod=1;
		trynum=trynum/10; 
		digit=0;
	}	
	return total;	 
}
