	#include<stdio.h>
	#include<math.h>
	int main()
	{
	int m;
    int n;	
	   printf("Enter the first number :: ");
       scanf("%d",&m);
	   printf("Enter the second number :: ");
       scanf("%d",&n);
	   //int m=0;
	   //int n=100;
	   int i=0;
	   int j=0;
	  
	  //int flag=0;
	  int d=0;
	  int p=0;
	  int x[10000];
	  int a[j];
	  int q=0;
	  int y[q];
	   
			 
	   
	   for(i=m;i<=n;i++)
	  { 
				//printf("Value going inside %d", i);
				int a[d];
				int num=i;
				d=0;
				 int w=0; //number of digits
				int flagzero=0;
				int flag=0;
		  if (i==0)
          {
          x[0]=0;
		  //printf("I am in else %d \n",p);
		  printf("INVALID %d \n",i);
		  p++;
		  }		  
		  while(num>0) //101  
		  { 
			a[w] = num%10;	 //1     
			//printf("a[d] %d",a[d]);   
			num = num/10;    //num=10    
			w++;  //increment number of digits
		  
		  }
		  for (int h=0;h<w;h++)  //111 [a(0)=1] 1
		  {
			  if(a[h]==0)
			  {
				  flagzero++;
				  x[p]=i;
				  printf("INVALID %d \n",i);
				  p++;
				  break;
			  }
		  }
		  
		  //printf("flagzero %d \n",flagzero);
		 
	   if(flagzero==0 && i != 0){
	   for(j=0;j<w;j++)
	   { 
		//	printf("number of digits %d \n",w);
		  // printf("value of i is %d\n",i);  
		   //printf("value of j is %d" ,j); 	   
		   //printf("a[j] %d /n",a[j]);  
		   if(i%a[j]==0)
		   {
			  //printf("digit is divisible by num\n %d",i);
		   
			  
			  flag++; 
		   }
	   }
		//printf("flag %d",flag);
		 if(flag==w){
		  //printf("q is %d",q);
		   printf("VALID NUMBER %d \n",i);
		  y[q]=i;
		  q++;
		  
				 }
		else
		{  
			//printf("value of i is %d \n",i);  
			//printf("I am in else %d \n",p);
			//printf("Do I have i here? %d \n",p=i);
			x[p]=i;
			printf("INVALID %d \n",x[p]);
			p++;
		}
	  }
	  }
	  
	}
	 
						
	 


