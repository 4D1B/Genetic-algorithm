package javaapplication21;

import static java.lang.Math.abs;

/**
 *
 * @author ADG
 */
public class JavaApplication21 {

    public static int func(int[] xx)
    {
        int x=0;
        x= abs((xx[0] + xx[1] )- (xx[2] +xx[3] ) + (xx[4] + xx[5]) - (xx[6] +xx[7]));
        return x;
    }
    
    public static void main(String[] args) {
        
        int x11 = 0,x22 = 0,x33 = 0,x44=0;
        float sum=0;
        int[] F ={0,0,0,0};
        
        
        float[] P = {0,0,0,0} ;
        int[] x1 = {5,2,1,3,4,9,7,8 };
        int[] x2 = {1,2,5,9,4,6,3,8 };
        int[] x3 = {5,6,7,8,9,1,2,3 };
        int[] x4 = {9,8,7,6,5,4,3,2 };
        
       // F[0] = abs((x1[0] + x1[1] )- (x1[2] +x1[3] ) + (x1[4] + x1[5]) - (x1[6] +x1[7]));
        F[0] = func(x1);
        F[1] = func(x2);
        F[2] = func(x3);
        F[3] = func(x4);
        
        
        
        for(int i =0 ; i<4;i++)
        {
            sum = sum + F[i];
        }
        
        System.out.println("Total fitness " + sum);
        System.out.println("Aavrg fitness " + sum/4);
        
        for(int i =0 ; i<4;i++)
        {
            P[i] = F[i] / sum;
            
        }
        
        float[] bin = {0,0,0,0};
        
        for(int i = 0 ;i<4;i++)
        {
            bin[i] = (float) Math.random();
        }
        
        for(int i =0,j=0;i<4;i++)
        {
            if(bin[i] >=0 && bin[i] < P[j])
            {
               if(i==0)
                {
                     x1= x1;
                }
                else if(i==1)
                {
                    x2=x1;
                }
                else if(i==2)
                {
                    x3=x1;
                }
                else if(i==3)
                {
                    x4=x1;
                }
            }
            else if(bin[i] >= P[j] && bin[i] < P[j+1] )
            {
                if(i==0)
                {
                     x1= x2;
                }
                else if(i==1)
                {
                    x2=x2;
                }
                else if(i==2)
                {
                    x3=x2;
                }
                else if(i==3)
                {
                    x4=x2;
                }
                   
            }
            else if(bin[i] >= P[j+1] && bin[i] < P[j+2] )
            {
                if(i==0)
                {
                     x1= x3;
                }
                else if(i==1)
                {
                    x2=x3;
                }
                else if(i==2)
                {
                    x3=x3;
                }
                else if(i==3)
                {
                    x4=x3;
                }
            }
            
            else if(bin[i] >= P[j+2] && bin[i] < P[j+3] )
            {
                if(i==0)
                {
                     x1= x4;
                }
                else if(i==1)
                {
                    x2=x4;
                }
                else if(i==2)
                {
                    x3=x4;
                }
                else if(i==3)
                {
                    x4=x4;
                }
            }
            
            
        }
        
      
        
     for(int i =0 ;i<4;i++)
     {
         int temp = x1[i+4];
         x1[i+4] = x3[i+4];
         x3[i+4] = temp;
     }
     
   
     
     x2[3] = 0;
     x3[3] = 0;
    
     for(int i=0;i<x1.length;i++)
     {
      
         System.out.print(x1[i] +" ");
        
     }
     
     
     
    F[0] = func(x1);
    F[1] = func(x2);
    F[2] = func(x3);
    F[3] = func(x4);
        
     
     
        for(int i =0 ; i<4;i++)
        {
            sum = sum + F[i];
        }
        
        
        
        System.out.println("Total fitness " + sum);
        System.out.println("Aavrg fitness " + sum/4);
        
        
        
        
        
    }
    
    

    
}

