# train-case-
2.package case1;
import java.util.*;

public class Case1 {

    
    public static void main(String[] args) {
        
         Scanner t=new Scanner(System.in);
         Scanner b1=new Scanner(System.in);
         String[][] Departuretimes=new String[3][15];
         String DepartureTimes[][]=new String[10][10];  
         int Passengersnumbers;
         int choice;
            String a[][]=new String[15][2];
       int b[]=new int[15];
       a[0][0]="\nMonday";
      a[0][1]="\t\t6.04";
       a[1][0]="\n";
       a[1][1]="9.04";
       a[2][1]="12.04";
       a[3][1]="15.04";
       a[4][1]="19.04";
       a[5][0]="\nTuesday";
       a[5][1]="\t\t6.04";
       a[6][0]="\0";
       a[6][1]="9.04";
       a[7][0]="\0";
       a[7][1]="12.04";
       a[2][0]="\0";
       a[3][0]="\0";
       a[4][0]="\0";
       a[1][0]="\0";
       a[8][0]="\0";
       a[8][1]="15.04";
       a[9][0]="\0";
       a[9][1]="19.04";
       a[14][0]="\0";
       a[13][0]="\0";
       a[11][0]="\0";
       a[12][0]="\0";
       a[10][0]="\nWednesday";
       a[10][1]="\t6.04";
       a[11][1]="9.04";
       a[12][1]="12.04";
       a[13][1]="15.04";
       a[14][1]="19.04";
        b[0]=22;
        b[1]=119;
        b[2]=64;
        b[3]=177;
        b[4]=21;
        b[5]=22;
        b[6]=111;
        b[7]=87;
        b[8]= 193;
        b[9]= 22;
        b[10]= 11;
        b[11]=107 ;
        b[12]= 93;
        b[13]= 162;
        b[14]= 42;
        
            
                
        System.out.println("Day \t\t\t\t\tDeparture Time \t\tNumber of Passenger");
        for(int i=0;i<15;i++)
        {
            for(int j=0;j<2;j++)
            {
            System.out.print("\t\t"+a[i][j] +"\t\t" );       
          
            }
            
                System.out.print(b[i]);
            
         System.out.println(""); 
        }
     System.out.println("\n\n1.)The most popular train (day and time)\n" +
"2.) Least popular train (day and time)\n" +
"3.) Whether 6.04 train is more popular than the 9.04 train\n" +
"4.) Whether 6.04 train on Monday is more popular than the 6.04 train on Tuesday\n" +
"5.) Which two trains is more popular where day and time is specified by the user\n" +
"6.) Display a list of all trains (day, time) where passenger numbers were below 50\n" +
"7.) Average number of passengers travelling on the 12.04 train over the three days (Monday, Tuesday, Wednesday)\n" +
"8.) Average number of passengers travelling where day and time is specified by the user\n"+
"9.)Exit");
         choice=t.nextInt();
        
         
         switch(choice)
         {
             case 1:
                 System.out.println("\t\tPopular train");
                 int pop=b[0];
                 for(int i=0;i<15;i++)
                 {
                     if(pop<b[i])
                     {
                         pop=b[i];
                     }
                 }
                 if(pop ==b[0] )
                         {
                          
                             System.out.println(a[0][0] + a[0][1]  );
                         }
                         else if(pop ==b[1])
                             System.out.println(a[0][0]+ a[1][1]);
                     else if(pop ==b[2])
                             System.out.println(a[0][0]+ a[2][1]);
                         else if(pop ==b[3])
                             System.out.println(a[0][0]+ a[3][1]);
                     else if(pop ==b[4])
                             System.out.println(a[0][0]+ a[4][1]);
                         else if(pop ==b[5])
                             System.out.println(a[5][0]+ a[5][1]);
                         else if(pop ==b[6])
                             System.out.println(a[5][0]+ a[6][1]);
                    else if(pop ==b[7])
                             System.out.println(a[5][0]+ a[7][1]);
                else if(pop ==b[8])
                             System.out.println(a[5][0]+ a[8][1]);
                         else if(pop ==b[9])
                             System.out.println(a[5][0]+ a[9][1]);
                         else if(pop ==b[10])
                             System.out.println(a[10][0]+ a[10][1]);
                     else if(pop ==b[11])
                             System.out.println(a[10][0]+ a[11][1]);
                     else if(pop ==b[12])
                             System.out.println(a[10][0]+ a[12][1]);
                    else if(pop ==b[13])
                             System.out.println(a[10][0]+ a[13][1]);
                         else if(pop ==b[14])
                             System.out.println(a[10][0]+ a[14][1]);
                // System.out.println("Day:\t"+ a[5][0]+"\n\nTime:\t"+ a[8][1]);
                 break ;
             case 2:
                 System.out.println("\t\tLeast Popular train");
                 int pop1=b[0];
                 for(int i=0;i<15;i++)
                 {
                     if(pop1>b[i])
                     {
                         pop1=b[i];
                     }
                 }
                 if(pop1 ==b[0] )
                         {
                    System.out.println(a[0][0] + a[0][1]  );
                         }
                         else if(pop1 ==b[1])
                             System.out.println(a[0][0]+ a[1][1]);
                     else if(pop1 ==b[2])
                             System.out.println(a[0][0]+ a[2][1]);
                         else if(pop1 ==b[3])
                             System.out.println(a[0][0]+ a[3][1]);
                     else if(pop1 ==b[4])
                             System.out.println(a[0][0]+ a[4][1]);
                         else if(pop1 ==b[5])
                             System.out.println(a[5][0]+ a[5][1]);
                         else if(pop1 ==b[6])
                             System.out.println(a[5][0]+ a[6][1]);
                    else if(pop1 ==b[7])
                             System.out.println(a[5][0]+ a[7][1]);
                 else if(pop1 ==b[8])
                             System.out.println(a[5][0]+ a[8][1]);
                         else if(pop1 ==b[9])
                             System.out.println(a[5][0]+ a[9][1]);
                         else if(pop1 ==b[10])
                             System.out.println(a[10][0]+ a[10][1]);
                     else if(pop1 ==b[11])
                             System.out.println(a[10][0]+ a[11][1]);
                     else if(pop1 ==b[12])
                             System.out.println(a[10][0]+ a[12][1]);
                    else if(pop1 ==b[13])
                             System.out.println(a[10][0]+ a[13][1]);
                         else if(pop1 ==b[14])
                             System.out.println(a[10][0]+ a[14][1]);
             // System.out.println("Day:\t" + a[10][0] +"\n\nTime:\t"+ a[10][1]);
                 break ;
             case 3:
                 System.out.println("Time:6.04 \nDay:Monday \tPassengers:22\n \nDay:Tuesday \tPassengers:22 \nDay:Wednesday \tPassengers:11");
                 System.out.println("Time:9.04 \nDay:Monday \tPassengers:119 \nDay:Tuesday \tPassengers:111 \nDay:Wednesday \tPassengers:107");
                 double t1=6.04,t2=9.04;
                 double p11=22,p12=22,p13=11,p21=119,p22=111,p23=107;
                 if(p11>p21 && p11>p22 && p11>p23 && p12>p21 && p12>p22 && p12>p23 && p13>p21 && p13>p22 && p13>p23)
                 {
                     System.out.println("6.04 train is popular");
                 }
                 else
                 {
                     System.out.println("9.04 train is popular");
                 }
                
                 break ;
             case 4:
                System.out.println("Both the trains are not popular");                 
                System.out.println("Monday \t\tTime:6.04 \nPassengers:22 \nTuesday \tTime:6.04 \nPassengers:22");
                int q=22,w=22;
                if(q>w)
                {
                System.out.println("Monday-train is popular");
                        }
                else
                    System.out.println("Both trains are equally popular");
                        break ;
             case 5:
                 
                   /*int ty[]={22,119,64,177,21 };
                   int ty1[]={22,111,87,193,22};
                   int ty2[]={11,107,93,162,42};
*/                   
double oi[]={6.04,9.04,12.04,15.04,19.04,6.04,9.04,12.04,15.04,19.04,6.04,9.04,12.04,15.04,19.04};
                   //double oi2[]={6.04,9.04,12.04,15.04,19.04};
                   //double oi3[]={6.04,9.04,12.04,15.04,19.04};
                   String lp[]=new String[3];
                   lp[0]="Monday";
                   lp[1]="Tuesday";
                   lp[2]="Wednesday";
                   String nm[]=new String[2];
                   int sum=0,sum1=0,sum2=0,total;
                   double oi1[]=new double[2];
                   for(int i=0;i<2;i++)
                   {
                   System.out.println("Enter the Day");
                   nm[i]=b1.nextLine();
                   
                   }
                   for(int i=0;i<2;i++)
                   {
                   System.out.println("Enter the time");
                   oi1[i]=t.nextDouble();
                   }
                  
                   
                   for(int i=0;i<2;i++)
                   {
                       
                       for(int j=0;j<5;j++)
                       {
                           if(nm[i].contentEquals(lp[0]))
                           {
                               if(oi1[i]==oi[j])
                               {
                                  sum=sum+b[j]; 
                               }
                               }
                       }
                   }
                    for(int i=0;i<2;i++)
                   {
                   
                       for(int j=5;j<10;j++)
                       {
                           if(nm[i].contentEquals(lp[1]))
                           {
                               if(oi1[i]==oi[j])
                               {
                                   
                                  sum1=sum1+b[j]; 
                               } 
                           }
                       }
                    }
                   
                     for(int i=0;i<2;i++)
                   {
                      
                           for(int j=10;j<15;j++)
                       {
                            if(nm[i].contentEquals(lp[2]))
                           {
                                if(oi1[i]==oi[j])
                               {
                                   
                                  sum2=sum2+b[j]; 
                               }
                           }
                       
                   }
                   }
                if(sum>sum1 &&sum>sum2)
                {
                    System.out.println("Train1 is popular");
                }
                else if(sum1>sum2)
                {
                     System.out.println("Train2 is popular");
                }
                else
                     System.out.println("Train3 is popular");
                 break ;
             case 6:
                  int pp[]={22,119,64,177,21 };
                   int pp1[]={22,111,87,193,22};
                   int pp2[]={11,107,93,162,42};
                   double oo1[]={6.04,9.04,12.04,15.04,19.04};
                   double oo2[]={6.04,9.04,12.04,15.04,19.04};
                   double oo3[]={6.04,9.04,12.04,15.04,19.04};
                   String  e1[]=new String[3];
                   e1[0]="Monday";
                   e1[1]="Tuesday";
                   e1[2]="Wednesday";
                   for(int i=0;i<3;i++)
                   {
                       for(int j=0;j<5;j++)
                       {
                           if(pp[j]<50)
                           {
                               System.out.println("Day: "+e1[i]+"\nTime: "+oo1[i]+"\nPassengers: "+pp[j]);
                           }
                           else if(pp1[j]<50)
                           {
                               System.out.println("Day: "+e1[i]+"\nTime: "+oo2[i]+"\nPassengers: "+pp1[j]);
                           }
                           else if(pp2[j]<50)
                           {
                               System.out.println("Day: "+e1[i]+"\nTime: "+oo3[i]+"\nPassengers: "+pp2[j]);
                           }
                       }
                   }
                 break ;
             case 7:
                  int g,y=64,m=87,n=93,d;
                 System.out.println("Monday \n\tPassengers:64 \nTuesday \n\tPassengers:87 \nWednesday \n\tPassengers:93");        
                 d=y+m+n;
                 System.out.println("The Average passengers: "+ d/3);
                 break;
             case 8:
                  int ty13[]={22,119,64,177,21 };
                   int ty11[]={22,111,87,193,22};
                   int ty12[]={11,107,93,162,42};
                   double oi111[]={6.04,9.04,12.04,15.04,19.04};
                   double oi12[]={6.04,9.04,12.04,15.04,19.04};
                   double oi13[]={6.04,9.04,12.04,15.04,19.04};
                   String lp1[]=new String[3];
                   lp1[0]="Monday";
                   lp1[1]="Tuesday";
                   lp1[2]="Wednesday";
                   String nm1;
                   int sum111=0,sum11=0,sum12=0,total1;
                   double oi11;
                  System.out.println("Enter the Day");
                   nm1=b1.nextLine();  
                   System.out.println("Enter the time");
                   oi11=t.nextDouble();
                  for(int j=0;j<5;j++)
                       {
                           if(nm1.contentEquals(lp1[0]))
                           {
                               if(oi11==oi111[j])
                               {
                   System.out.println("The average passengers:"+ty13[j]); 
                               }
                               }
                           else if(nm1.contentEquals(lp1[1]))
                           {
                               if(oi11==oi12[j])
                               {
                                  System.out.println("The average passengers:"+ty11[j]); 
                               } 
                           }
                           else if(nm1.contentEquals(lp1[2]))
                           {
                                if(oi11==oi13[j])
                               {
                                System.out.println("The average passengers"+ty12[j]); 
                               }
                           }
                       }
                   
                
                   break ;                 
             case 9:
                
               System.exit(0); 
             default:
                 System.out.println("\nInvalid!!");
                 
     }
        
}
}

