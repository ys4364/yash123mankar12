#include <stdio.h> 
int main()                                                                                                                                                                                                                                   
{ int talktime;          
float bill; 
printf("Enter number of talktime :"); 
scanf("%d", &talktime); 
if (talktime <= 100) { bill = 200; 
}
else if (talktime > 100 && talktime<= 150) 
{
 talktime = talktime - 100; 
bill = 200+(0.60 *talktime); 
} 
else if (talktime> 150 && talktime<= 200) 
{ 
talktime = talktime - 150; bill = 200+(0.60 *50) + (0.50 *talktime);
 } 
else 
{ 
talktime = talktime - 200; 
bill = 200 + (0.60 * 50) + (0.50 * 50) + (0.40 * talktime); 
}
printf("Your bill is Rs. %0.2f", bill);
return 0; 
}
