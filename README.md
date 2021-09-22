# let-us-c-6
Q.(f) Paper of size A0 has dimensions 1189 mm x 841 mm. Each subsequent size A(n) is defined as A(n-1) cut in half parallel to its shorter sides. Write a program to calculate and print paper sizes A0, A1, A2, ….. A8.


     #include<stdio.h>
     int main()
    {
         
        int p=0;
        float x=1189.0,y=841.0,temp;
        temp=x;

           while(p<11) 
      {     
         
   	    printf("A%d = %.1fmm * %.1fmm\n\n",p,x,y);
   	    x= y;
   	    y= temp/2;
   	    temp = x;
        p=p+1;
	   }
	
    }
