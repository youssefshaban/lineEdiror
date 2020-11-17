#include<stdio.h>
#include<string.h>
#include<conio.h>
void Print (char ar[]);
int main (){
	char ar[41];
	char input;
	int lastIndex=0;
	int flag=0;
	int currentPosition = 0;
	clrscr();
	gotoxy(1,1);
	while(flag == 0){
	      input = getch();
		if (input == 0){
			input=getch();
			if(input == 77){
				if(currentPosition < lastIndex){
				currentPosition ++;
				gotoxy(currentPosition+1,1);
				}
			}
		      else if(input == 75){
				if(currentPosition > 0){
				currentPosition -- ;
				gotoxy(currentPosition+1,1);
				}
			}
		       else if(input == 71){
				currentPosition = 0;
				gotoxy(currentPosition+1,1);
			}
			else if(input == 79){
				currentPosition = lastIndex;
				gotoxy(currentPosition+1,1);
			}

	      }else {
		if(input == 13){

			ar[lastIndex]=0;
			gotoxy(10,15);
			printf("%s",ar);
			getch();
			flag=1;
		}
		else if(input == 27){
			ar[0]=0;
			flag = 1 ;
		}
		else if(isprint(input)!=0 && currentPosition<40 ){

			ar[currentPosition]=input;
			gotoxy(currentPosition+1, 1);
			printf("%c", ar[currentPosition]);
			if (lastIndex==currentPosition){
				lastIndex++;
				ar[lastIndex]=0 ;
			}

			currentPosition ++;

			gotoxy(currentPosition+1,1);
		}


	      }

	}





	return 0 ;

}

void Print (char ar[]){
	clrscr();
	printf("%s",ar);

}
