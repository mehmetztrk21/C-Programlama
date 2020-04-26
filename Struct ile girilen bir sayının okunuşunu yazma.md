# C-Programlama
C Programlama İleri Düzey Örnekler
#include <stdio.h>
#include <stdlib.h>

/* run this program using the console pauser or add your own getch, system("pause") or input loop */

struct Sayi{
	
	int sayi;
	char yuzbinler_yuzler[9][10];
	char onbinler_onlar[9][10];
	char binler[9][10];
	char birler[9][10];


	
};



int main(int argc, char *argv[]) {
	struct Sayi x={1,{"yuz","iki yuz","uc yuz","dort yuz","bes yuz","alti yuz","yedi yuz","sekiz yuz","dokuz yuz"},
	{"on","yirmi","otuz","kirk","elli","altmis","yetmis","seksen","doksan"},
	{"bin","iki bin","uc bin","dort bin","bes bin","alti bin","yedi bin","sekiz bin","dokuz bin"},
	{"bir","iki","uc","dort","bes","alti","yedi","sekiz","dokuz"}};
		
	while(1>0){
	
	printf("0-999999 arasinda bir sayi giriniz:");
	scanf("%d",&x.sayi);
	
	if(x.sayi==0)	printf("Girilen sayinin okunusu:sifir\n");
	
	else if((x.sayi<999999 && x.sayi>0) || (x.sayi>=-999999 && x.sayi<0)){
	
	if(x.sayi>0)	printf("Girilen sayinin okunusu:");
	
	else{
		printf("Girilen sayinin okunusu:eksi ");
		x.sayi=x.sayi*(-1);
	}
		
		//yüzbinler
		if(x.sayi/100000==1)		printf("%s",x.yuzbinler_yuzler[0]);
		
		else if(x.sayi/100000==2)	printf("%s",x.yuzbinler_yuzler[1]);
	
		else if(x.sayi/100000==3)	printf("%s",x.yuzbinler_yuzler[2]);
		
		else if(x.sayi/100000==4)	printf("%s",x.yuzbinler_yuzler[3]);
		
		else if(x.sayi/100000==5)	printf("%s",x.yuzbinler_yuzler[4]);
		
		else if(x.sayi/100000==6)	printf("%s",x.yuzbinler_yuzler[5]);
		
		else if(x.sayi/100000==7)	printf("%s",x.yuzbinler_yuzler[6]);
			
		else if(x.sayi/100000==8)	printf("%s",x.yuzbinler_yuzler[7]);
			
		else if(x.sayi/100000==9)	printf("%s",x.yuzbinler_yuzler[8]);
		
		
		//onbinler
		if((x.sayi%100000)/10000==1)		printf(" %s",x.onbinler_onlar[0]);
		
		else if((x.sayi%100000)/10000==2)	printf(" %s",x.onbinler_onlar[1]);
			
		else if((x.sayi%100000)/10000==3)	printf(" %s",x.onbinler_onlar[2]);
		
		else if((x.sayi%100000)/10000==4)	printf(" %s",x.onbinler_onlar[3]);
		
		else if((x.sayi%100000)/10000==5)	printf(" %s",x.onbinler_onlar[4]);
		
		else if((x.sayi%100000)/10000==6)	printf(" %s",x.onbinler_onlar[5]);
		
		else if((x.sayi%100000)/10000==7)	printf(" %s",x.onbinler_onlar[6]);
		
		else if((x.sayi%100000)/10000==8)	printf(" %s",x.onbinler_onlar[7]);
		
		else if((x.sayi%100000)/10000==9)	printf(" %s",x.onbinler_onlar[8]);
		
		
		//binler
		if(((x.sayi%100000)/1000)%10==1)		printf(" %s",x.binler[0]);
		
		else if(((x.sayi%100000)/1000)%10==2)	printf(" %s",x.binler[1]);
		
		else if(((x.sayi%100000)/1000)%10==3)	printf(" %s",x.binler[2]);
	
		else if(((x.sayi%100000)/1000)%10==4)	printf(" %s",x.binler[3]);
		
		else if(((x.sayi%100000)/1000)%10==5)	printf(" %s",x.binler[4]);
		
		else if(((x.sayi%100000)/1000)%10==6)	printf(" %s",x.binler[5]);
		
		else if(((x.sayi%100000)/1000)%10==7)	printf(" %s",x.binler[6]);
		
		else if(((x.sayi%100000)/1000)%10==8)	printf(" %s",x.binler[7]);
		
		else if(((x.sayi%100000)/1000)%10==9)	printf(" %s",x.binler[8]);
		
		else{				
			if(x.sayi>1000)
			printf(" bin");
			}
		
		
		//yüzler
		if((x.sayi%1000)/100==1)		printf(" %s",x.yuzbinler_yuzler[0]);
		
		else if((x.sayi%1000)/100==2)	printf(" %s",x.yuzbinler_yuzler[1]);
		
		else if((x.sayi%1000)/100==3)	printf(" %s",x.yuzbinler_yuzler[2]);
		
		else if((x.sayi%1000)/100==4)	printf(" %s",x.yuzbinler_yuzler[3]);
		
		else if((x.sayi%1000)/100==5)	printf(" %s",x.yuzbinler_yuzler[4]);
		
		else if((x.sayi%1000)/100==6)	printf(" %s",x.yuzbinler_yuzler[5]);
		
		else if((x.sayi%1000)/100==7)	printf(" %s",x.yuzbinler_yuzler[6]);
		
		else if((x.sayi%1000)/100==8)	printf(" %s",x.yuzbinler_yuzler[7]);
		
		else if((x.sayi%1000)/100==9)	printf(" %s",x.yuzbinler_yuzler[8]);
		
		
		//onlar
		if((x.sayi%100)/10==1)			printf(" %s",x.onbinler_onlar[0]);
		
		else if((x.sayi%100)/10==2)		printf(" %s",x.onbinler_onlar[1]);
		
		else if((x.sayi%100)/10==3)		printf(" %s",x.onbinler_onlar[2]);
		
		else if((x.sayi%100)/10==4)		printf(" %s",x.onbinler_onlar[3]);
		
		else if((x.sayi%100)/10==5)		printf(" %s",x.onbinler_onlar[4]);
		
		else if((x.sayi%100)/10==6)		printf(" %s",x.onbinler_onlar[5]);
		
		else if((x.sayi%100)/10==7)		printf(" %s",x.onbinler_onlar[6]);
		
		else if((x.sayi%100)/10==8)		printf(" %s",x.onbinler_onlar[7]);
		
		else if((x.sayi%100)/10==9)		printf(" %s",x.onbinler_onlar[8]);
		
		
		//birler
		if(x.sayi%10==1)	printf(" %s",x.birler[0]);
		
		else if(x.sayi%10==2)	printf(" %s",x.birler[1]);
		
		else if(x.sayi%10==3)	printf(" %s",x.birler[2]);
		
		else if(x.sayi%10==4)	printf(" %s",x.birler[3]);
		
		else if(x.sayi%10==5)	printf(" %s",x.birler[4]);
		
		else if(x.sayi%10==6)	printf(" %s",x.birler[5]);
		
		else if(x.sayi%10==7)	printf(" %s",x.birler[6]);
		
		else if(x.sayi%10==8)	printf(" %s",x.birler[7]);
		
		else if(x.sayi%10==9)	printf(" %s",x.birler[8]);
		
	
		printf("\n");
	}
	
	else	printf("Lutfen belirtilen aralikta bir sayi giriniz...\n");
		
}
		
	return 0;
}
