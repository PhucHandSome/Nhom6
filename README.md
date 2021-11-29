#include<stdio.h>
main(){
	int n;
	printf(" nhap vao gia tri n   ");
	scanf("%d", &n);
	int a[n];
	for (int i=0; i<n; i++){
	printf("nhap vao a[%d]  ", i);
	scanf("%d", &a[i]);
	}
	for (int j=0; j<n; j++)
	for ( int i=0; i<n-1; i++)
	{
		int hv;
		if(a[i]>a[i+1])
		{
			hv=a[i];
			a[i]=a[i+1];
			a[i+1]=hv;
			}
			}
			printf("mang da sap xep la \n");
			for (int i=0; i<n; i++){
				printf("%d  ", a[i]);
				
			}
			}
