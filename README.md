# pizza.java
package session2;
import java.util.*;
import java.util.Scanner;
public class PizzaMania {
	public static void main(String[] args) {
				int t1=0,a=0,b,c,d,e,f,g,h,i,j,k,l,m,n,o,p,q,r,s,t,u,v,w,x,y,z;
				float a1;
				Scanner sc=new Scanner(System.in);
				String name=" ",s1,s2;
			    Vector v1=new Vector(10,4);
				Vector v2=new Vector(10,4);
				System.out.println("HIIII WHATS UR NAME ");
				name=sc.nextLine();
			    System.out.println("                                                     'WELCOME TO PIZZA MANIA'                                            ");
				System.out.println("");
				while(a!=3)
				{
					if(a==1||a==2)
					{
						System.out.println("ENTER 3 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE PIZZA or BEVERAGES...");
						System.out.println("");
					}  
				System.out.println("WHAT DO U WANT:\n1.PIZZA\n2.BEVERAGES\n3.EXIT\n");
				System.out.println("ENTER UR CHOICE:");
			    a=sc.nextInt();
			    System.out.println("");
				switch(a)	
				{
				case 1:	System.out.println("            PIZZA                           ");
						System.out.println("");
						b=0;
					while(b!=3)
					{
						if(b==1||b==2)
						{
							System.out.println("ENTER 3 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE VEG OR NON VEG PIZZA...");
							System.out.println("");
						}
						System.out.println("WHICH ONE DO U WANT?");
						System.out.println("1.VEG PIZZA\n2.NON-VEG PIZZA\n3.EXIT");
						System.out.println("ENTER UR CHOICE:");
						b=sc.nextInt();
						System.out.println("");
				       if(b==1)
				       {
				    	   c=0;
				    	   while(c!=6)
				    	   {
				    		   if(c==1||c==2||c==3||c==4||c==5)
								{
									System.out.println("ENTER 6 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE VEG PIZZA...");
									System.out.println("");
								}
				    	System.out.println("");
						System.out.println("              [VEG PIZZA]                           ");
						System.out.println("");
						System.out.println("SrNo NAME                      RATE");
						System.out.println("1.   SWEET CORN                100\n2.   PEPPY PANNER              120\n3.   MEXICAN DELIGHT           140\n4.   VEGGIE\n     PARADISE                  200\n5.   MARGHERITA                300\n6.   EXIT");
						System.out.println("ENTER UR CHOICE:");
						c=sc.nextInt();
						System.out.println("");
						switch(c)
						{
						case 1:t1+=100;
						       v2.addElement(new Integer(100));
						       v1.addElement(new String ("VEG PIZZA=SWEET CORN"));
							  	break;
						case 2:t1+=120;
						 v2.addElement(new Integer(120));
							   	v1.addElement(new String("VEG PIZZA=PEPPY PANNER"));
								break;
						case 3:t1+=140;
						 v2.addElement(new Integer(140));
						 		v1.addElement(new String("VEG PIZZA=MEXICAN DELIGHT"));
								break;
						case 4:t1+=200;
						 v2.addElement(new Integer(200));	
								v1.addElement(new String("VEG PIZZA=VEGGIE \nPARADISE"));
								break;
						case 5:t1+=300;
						 v2.addElement(new Integer(300));
								v1.addElement(new String("VEG PIZZA=MARGHERITA"));
								break;
						case 6:System.out.println("EXITED");
						System.out.println("");
							break;	
						default:System.out.println("SORRY INVALID CHOICE...");
						}	
					 if(c==1||c==2||c==3||c==4||c==5)
					 {
						 d=0;
						 while(d!=1&&d!=2&&d!=3)
						 {
						 System.out.println("WHAT WILL BE THE SIZE?");
						 System.out.println("              [SIZE]                                                          ");
						 System.out.println("SrNo SIZE                     RATE");
						 System.out.println("1.   SMALL                    5\n2.   MEDIUM                   10\n3.   LARGE                    15");
						 System.out.println("ENTER YOUR CHOICE:");
						 d=sc.nextInt();
						 System.out.println("");
					switch(d)
					{
					case 1:t1+=5;
					 v1.addElement(new String ("SIZE=SMALL"));
					 v2.addElement(new Integer(5));
					 break;
					case 2:t1+=10;
					 v1.addElement(new String ("SIZE=MEDIUM"));
					 v2.addElement(new Integer(10));
						break;
					case 3:t1+=15;
					 v1.addElement(new String ("SIZE=LARGE"));
					 v2.addElement(new Integer(15));
											break;
					default:System.out.println("SORRY INVALID CHOICE...");
					System.out.println("PLZZ ENTER THE OTHER OPTIONS FOR SIZE");
					System.out.println("U CAN SELECT THE OPTIONS FROM 1,2&3");
					
					}	
						 }
						 e=0;
						 while(e!=1&&e!=2&&e!=3)
						 {
				System.out.println("WHICH TYPE OF CRUST DO U WANT?");
				System.out.println("");
				System.out.println("               [CRUST]          ");
				System.out.println("SrNo CRUST                     RATE");
				System.out.println("1.   THIN                      25\n2.   THICK                     50\n3.   CHEESE                    75");
				System.out.println("Enter your choice:");
				e=sc.nextInt();
				System.out.println("");
				switch(e)
				{
				case 1:t1+=25;
					v1.addElement(new String("CRUST=THIN"));
					v2.addElement(new Integer(25));
					break;
				case 2:t1+=50;
					v1.addElement(new String ("CRUST=THICK"));
					 v2.addElement(new Integer(50));
					break;
				case 3:t1+=75;
				 v1.addElement(new String ("CRUST=CHEESE"));
				 v2.addElement(new Integer(75));
					break;
				default:System.out.println("SORRY INVALID CHOICE...");
				System.out.println("PLZZ ENTER THE OTHER OPTIONS FOR CRUST");
				System.out.println("U CAN SELECT THE OPTIONS FROM 1,2&3");
					   }
					 }		 
				f=0;
				while(f!=4)
				{
					if(f==1||f==2||f==3)
					{
						System.out.println("ENTER 4 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE TOPPINGS...");
						System.out.println("");
					}	
				System.out.println("WHAT WILL BE UR TOPPINGS?");
				System.out.println("");
				System.out.println("                [TOPPINGS]             ");
				System.out.println("SrNo TOPPINGS                  RATE");
				System.out.println("1.   TOMATO                    15\n2.   ONION                     20\n3.   OLIVES                    30\n4.   EXIT");
				System.out.println("ENTER UR CHOICE");
				f=sc.nextInt();
				System.out.println("");
				switch(f)
				{
				case 1:t1+=15;
						v1.addElement(new String("TOPPINGS=TOMATO")); 
						v2.addElement(new Integer(15));
				break;
				case 2:t1+=20;
						v1.addElement(new String("TOPPINGS=ONION"));
						v2.addElement(new Integer(20));
				break;
				case 3:t1+=30;
						v1.addElement(new String("TOPINGS=OLIVES")); 
						v2.addElement(new Integer(30));
				break;
				case 4:	System.out.println("EXICTED");
						System.out.println("");
				break;
				default:System.out.println("SORRY INVALID CHOICE...");
			   }
				}
					 }
								}
				}
				else if(b==2)
				{
					g=0;
					while(g!=6)
					{
						if(g==1||g==2||g==3||g==4||g==5)
						{
							System.out.println("ENTER 6 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE NON VEG PIZZA...");
							System.out.println("");
						}
						System.out.println("            [NON-VEG PIZZA]          ");
						System.out.println("SrNo NAME                      RATE");
						System.out.println("1.   BBQ CHICKEN               200\n2.   CHI TIKKA                 220\n3.   CHI FEAST                 240\n4.   BUTTER CHI                400\n5.   PIZZAMANIA DELIGHT        600\n6.   EXIT");
						System.out.println("ENTER UR CHOICE:");
						g=sc.nextInt();
						System.out.println("");
						switch(g)
							{
							case 1:t1+=200;
							 	v1.addElement(new String ("NON-VEG PIZZA=BBQ CHICKEN"));
							 	v2.addElement(new Integer(200));
							break;
							case 2:t1+=220;
							 	v1.addElement(new String ("NON-VEG PIZZA=CHI TIKKA"));
							 	v2.addElement(new Integer(220));
							break;
							case 3:t1+=240;
							 	v1.addElement(new String ("NON-VEG PIZZA=CHI FEAST"));
							 	v2.addElement(new Integer(240));
							break;
							case 4:t1+=400;
							 	v1.addElement(new String ("NON-VEG PIZZA=BUTTER CHI"));
							 	v2.addElement(new Integer(400));
							break;
							case 5:t1+=600;
							 	v1.addElement(new String ("NON-VEG PIZZA=PIZZAMANIA DELIGHT"));
							 	v2.addElement(new Integer(600));
							break;
							case 6:System.out.println("EXITED");
							System.out.println("");
							break;
							default:System.out.println("SORRY INVALID CHOICE...");
						   }
					 if(g==1||g==2||g==3||g==4||g==5)
					 {
						 h=0;
						 while(h!=1&&h!=2&&h!=3)
						 {
						 System.out.println("WHAT WILL BE THE SIZE?");
						 System.out.println("");
						 System.out.println("              [SIZE]                                                          ");
						 System.out.println("SrNo SIZE                     RATE");
						 System.out.println("1.   SMALL                    5\n2.   MEDIUM                   10\n3.   LARGE                    15");
						 System.out.println("ENTER UR CHOICE:");
						 h=sc.nextInt();
						 System.out.println("");
					switch(h)
					{
					case 1:t1+=5;
					 	v1.addElement(new String ("SIZE=SMALL"));
					 	v2.addElement(new Integer(5));
					break;
					case 2:t1+=10;
					 	v1.addElement(new String ("SIZE=MEDIUM"));
					 	v2.addElement(new Integer(10));					
					break;
					case 3:t1+=15;
					 	v1.addElement(new String ("SIZE=LARGE"));
					 	v2.addElement(new Integer(15));
					break;
					default:System.out.println("SORRY INVALID CHOICE...");
					System.out.println("PLZZ ENTER THE OTHER OPTIONS FOR SIZE");
					System.out.println("U CAN SELECT THE OPTIONS FROM 1,2&3");
						   }
						 }
						 i=0;
						 while(i!=1&&i!=2&&i!=3)
						 {
				System.out.println("WHICH TYPE OF CRUST DO U WANT?");
				System.out.println("");
				System.out.println("                  [CRUST]                                                          ");
				System.out.println("SrNo CRUST                     RATE");
				System.out.println("1.   THIN                      25\n2.   THICK                     50\n3.   CHEESE                    75");
				System.out.println("ENTER UR CHOICE:");
				i=sc.nextInt();
				System.out.println("");
				switch(i)
				{
				case 1:t1+=25;
					v1.addElement(new String ("CRUST=THIN"));
					v2.addElement(new Integer(25));
				break;
				case 2:t1+=50;
				 	v1.addElement(new String ("CRUST=THICK"));
				 	v2.addElement(new Integer(50));
				break;
				case 3:t1+=75;
				 	v1.addElement(new String ("CRUST=CHEESE"));
				 	v2.addElement(new Integer(75));
				break;
				default:System.out.println("SORRY INVALID CHOICE...");
				System.out.println("PLZZ ENTER THE OTHER OPTIONS FOR CRUST");
				System.out.println("U CAN SELECT THE OPTIONS FROM 1,2&3");
					   }
					 }
				j=0;
				while(j!=4)
				{
					if(j==1||j==2||j==3)
					{
						System.out.println("ENTER 4 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE TOPPINGS...");
						System.out.println("");
					}
				System.out.println("WHAT WILL BE UR TOPPINGS?");
				System.out.println("");
				System.out.println("                 [TOPPINGS]                                                          ");
				System.out.println("SrNo TOPPINGS                  RATE");
				System.out.println("1.   TOMATO                    15\n2.   ONION                     20\n3.   OLIVE                     30\n4.   Exit");
				System.out.println("ENTER UR CHOICE:");
				j=sc.nextInt();
				System.out.println("");
				switch(j)
				{
				case 1:t1+=15;
					v1.addElement(new String ("TOPPINGS=TOMATO"));
					v2.addElement(new Integer(15));
				break;
				case 2:t1+=20;
					v1.addElement(new String ("TOPPINGS=ONION"));
					v2.addElement(new Integer(20));
				break;
				case 3:t1+=30;
					v1.addElement(new String ("TOPPINGS=OLIVE"));
					v2.addElement(new Integer(30));
				break;
				case 4:break;
				default:System.out.println("SORRY INVALID CHOICE...");
			   }
				}
					 }
				   }
				}
				   }
		       			break;
				case 2:System.out.println("              BEVERAGES                   ");  	
					k=0;
					while(k!=3)
					{
						if(k==1||k==2)
						{
							System.out.println("ENTER 3 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE HOT OR COLD BEVERAGES...");
							System.out.println("");
						}
				  		System.out.println("1.HOT BEVERAGES\n2.COLD BEVERAGES\n3.EXIT");
					      k=sc.nextInt();
					      System.out.println("");
				       if(k==1)
				       {
				    	 l=0;
				        while(l!=4)
					     {
				        	if(l==1||l==2||l==3)
							{
								System.out.println("ENTER 4 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE HOT BEVERAGES...");
								System.out.println("");
							}
					      System.out.println("             [HOT BEVERAGES]       ");
					      System.out.println("SrNo NAME                      RATE");
					      System.out.println("1.   TEA                       --\n2.   COFFEE                    --\n3.   CHOCO LAVA CAKE           100\n4.   EXIT");
					      System.out.println("Enter your choice:");
					      l=sc.nextInt();
					      System.out.println("");
					      switch(l)
							{
							case 1:System.out.println("THE FOLLOWING R THE OPTONS AVAILABLE FOR TEA");
							q=0;
							while(q!=5)
							{
								if(q==1||q==2||q==3||q==4)
								{
									System.out.println("ENTER 5 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE TEA...");
									System.out.println("");
								}	
							System.out.println("WHICH TEA DO U WANT?");
							System.out.println("");
							System.out.println("               [TEA]           ");
							System.out.println("SrNo TEA                  RATE");
							System.out.println("1.   GREEN TEA            15\n2.   BLACK TEA            20\n3.   LEOMEN TEA           30\n4.   MASALA TEA           40\n5.   EXIT");
							System.out.println("ENTER UR CHOICE");
							q=sc.nextInt();
							System.out.println("");
							switch(q)
							{
							case 1:t1+=15;
							    v1.addElement(new String("TEA=GREEN TEA"));
							    v2.addElement(new Integer(15));
								break;
							case 2:t1+=20;
								v1.addElement(new String("TEA=BLACK TEA")); 
								v2.addElement(new Integer(20));
								break;
							case 3:t1+=30;
						        v1.addElement(new String("TEA=LEOMEN TEA"));
								v2.addElement(new Integer(30));
								break;
							case 4:t1+=40;
								v1.addElement(new String("TEA=MASALA TEA"));
								v2.addElement(new Integer(40));
								break;
							case 5:System.out.println("EXICTED");
							System.out.println("");
								break;
							default:System.out.println("SORRY INVALID CHOICE...");
						   }
							      }
							 		  	break;
							case 2:System.out.println("THE FOLLOWING R THE OPTONS AVAILABLE FOR COFFEE");
							r=0;
							while(r!=4)
							{
								if(r==1||r==2||r==3)
								{
									System.out.println("ENTER 4 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE COFFEE...");
									System.out.println("");
								}	
							System.out.println("WHICH COFFEE DO U WANT?");
							System.out.println("");
							System.out.println("               [COFFEE]        ");
							System.out.println("SrNo COFFEE                  RATE");
							System.out.println("1.   BLACK COFFEE            15\n2.   CAPPUCCINO              20\n3.   ESPRESSO                30\n4.   EXIT");
							System.out.println("ENTER UR CHOICE");
							r=sc.nextInt();
							System.out.println("");
							switch(r)
							{
							case 1:t1+=15;
								v1.addElement(new String("COFFEE=BLACK COFFEE"));
								v2.addElement(new Integer(15));
								break;
							case 2:t1+=20;
								v1.addElement(new String("COFFEE=CAPPUCCINO")); 
								v2.addElement(new Integer(20));
								break;
							case 3:t1+=30;
								v1.addElement(new String("COFFEE=ESPRESSO")); 
								v2.addElement(new Integer(30));
								break;
							case 4:System.out.println("EXICTED");
							System.out.println("");
								break;
							default:System.out.println("SORRY INVALID CHOICE...");
						   }
								   }
									break;
							case 3:t1+=100;
							 v1.addElement(new String ("CHOCO LAVA CAKE"));
							 m=0;
							 while(m!=1&&m!=2&&m!=3)
							 {
							    System.out.println("WHAT WILL BE THE SIZE?");
								System.out.println("                [SIZE]    ");
								System.out.println("SrNo SIZE                     RATE");
								System.out.println("1.   SMALL                    5\n2.   MEDIUM                   10\n3.   LARGE                    15");
								System.out.println("ENTER UR CHOICE:");
								m=sc.nextInt();
						     switch(m)
							{
							case 1:t1+=5;
							 	v1.addElement(new String ("SIZE=SMALL"));
							 	v2.addElement(new Integer(5));
								break;
							case 2:t1+=10;
							 	v1.addElement(new String ("SIZE=MEDIUM"));
							 	v2.addElement(new Integer(10));
								break;
							case 3:t1+=15;
							 	v1.addElement(new String ("SIZE=LARGE"));
							 	v2.addElement(new Integer(15));
								break;
							default:System.out.println("SORRY INVALID CHOICE...");
							System.out.println("PLZZ ENTER THE OTHER OPTIONS FOR SIZE");
							System.out.println("U CAN SELECT THE OPTIONS FROM 1,2&3");
							}
							  } 
									break;
							case 4:System.out.println("EXITED");
							       System.out.println("");
								break;
							default:System.out.println("SORRY INVALID CHOICE...");
							}	
									}
				}
				else if(k==2)
				{
					n=0;
					while(n!=5)
					{
						if(n==1||n==2||n==3||n==4)
						{
							System.out.println("ENTER 5 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE COLD BEVERAGES...");
							System.out.println("");
						}
						System.out.println("            [COLD BEVERAGES]     ");
						System.out.println("SrNo NAME                      RATE");
						System.out.println("1.   SOFT DRINKS               --\n2.   ICE CREAMS                --\n3.   THICK SHAKES              --\n4.   COLD COFFEE               80\n5.   EXIT");
						System.out.println("ENTER UR CHOICE:");
						n=sc.nextInt();
						System.out.println("");
						switch(n)
						{
						case 1:System.out.println("THE FOLLOWING R THE OPTONS AVAILABLE FOR SOFT DRINKS");
						t=0;
						while(t!=5)
						{
							if(t==1||t==2||t==3||t==4)
							{
								System.out.println("ENTER 5 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE SOFT DRINKS...");
								System.out.println("");
							}	
						System.out.println("WHICH SOFT DRINK DO U WANT?");
						System.out.println("");
						System.out.println("                   [SOFT DRINKS]  ");
						System.out.println("SrNo SOFT DRINKS                  RATE");
						System.out.println("1.   MIRANDA                      15\n2.   PEPSI                        20\n3.   SEVEN UP                     30\n4.   THUMPS UP                    40\n5.   EXIT");
						System.out.println("ENTER UR CHOICE");
						t=sc.nextInt();
						System.out.println("");
						switch(t)
						{
						case 1:t1+=15;
							v1.addElement(new String("SOFT DRINKS=MIRANDA"));
							v2.addElement(new Integer(15));
							break;
						case 2:t1+=20;
							v1.addElement(new String("SOFT DRINKS=PEPSI")); 
							v2.addElement(new Integer(20));
							break;
						case 3:t1+=30;						
							v1.addElement(new String("SOFT DRINKS=SEVEN UP"));
							v2.addElement(new Integer(30));
							break;
						case 4:t1+=40;
							v1.addElement(new String("SOFT DRINKS=THUMS UP"));
							v2.addElement(new Integer(40));
							break;
						case 5:System.out.println("EXICTED");
						System.out.println("");
							break;
						default:System.out.println("SORRY INVALID CHOICE...");
					   }
						if(t==1||t==2||t==3||t==4)
						{
							 u=0;
							 while(u!=1&&u!=2&&u!=3)
							 {
						System.out.println("WHAT WILL BE THE SIZE?");
						System.out.println("                [SIZE]     ");
						System.out.println("SrNo SIZE                     RATE");
						System.out.println("1.   SMALL                    5\n2.   MEDIUM                   10\n3.   LARGE                    15");
						System.out.println("ENTER UR CHOICE:");
						u=sc.nextInt();
						System.out.println("");
				     switch(u)
					{
					case 1:t1+=5;
					 	v1.addElement(new String ("SIZE=SMALL"));
					 	v2.addElement(new Integer(5));
						break;
					case 2:t1+=10;
					 	v1.addElement(new String ("SIZE=MEDIUM"));
					 	v2.addElement(new Integer(10));
						break;
					case 3:t1+=15;
					 	v1.addElement(new String ("SIZE=LARGE"));
					 	v2.addElement(new Integer(15));
						break;
					default:System.out.println("SORRY INVALID CHOICE...");
					System.out.println("PLZZ ENTER THE OTHER OPTIONS FOR SIZE");
					System.out.println("U CAN SELECT THE OPTIONS FROM 1,2&3");
					}
				       }
					     }
						}
						 break;
						case 2:System.out.println("THE FOLLOWING R THE OPTONS AVAILABLE FOR ICE CREAMS");
						v=0;
						while(v!=5)
						{
							if(v==1||v==2||v==3||v==4)
							{
								System.out.println("ENTER 5 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE ICE CREAMS...");
								System.out.println("");
							}	
						System.out.println("WHICH ICECREAMS DO U WANT?");
						System.out.println("");
						System.out.println("                   [ICECREAMS]   ");
						System.out.println("SrNo ICECREAMS                  RATE");
						System.out.println("1.   VANILLA                    15\n2.   CHOCOLATE                  20\n3.   STRAWBERRY                 30\n4.   MANGO                      40\n5.   EXIT");
						System.out.println("ENTER UR CHOICE");
						v=sc.nextInt();
						System.out.println("");
						switch(v)
						{
						case 1:t1+=15;
							v1.addElement(new String("ICECREAM=VANILLA")); 
							v2.addElement(new Integer(15));
							break;
						case 2:t1+=20;
							v1.addElement(new String("ICECREAM=CHOCOLATE"));
							v2.addElement(new Integer(20));
							break;
						case 3:t1+=30;
							v1.addElement(new String("ICECREAM=STRAWBERRY"));
							v2.addElement(new Integer(30));
							break;
						case 4:t1+=40;
							v1.addElement(new String("ICECREAM=MANGO"));
							v2.addElement(new Integer(40));
							break;
						case 5:System.out.println("EXICTED");
						System.out.println("");
							break;
						default:System.out.println("SORRY INVALID CHOICE...");
					   }
						}
						 break;
						case 3:System.out.println("THE FOLLOWING R THE OPTONS AVAILABLE FOR THICK SHAKES");
						x=0;
						while(x!=5)
						{
							if(x==1||x==2||x==3||x==4)
							{
								System.out.println("ENTER 5 IF U WANT TO EXIT OR ENETR THE OTHER OPTIONS IF U WANT MORE THICK SHAKES...");
								System.out.println("");
							}	
						System.out.println("WHICH SHAKE DO U WANT?");
						System.out.println("");
						System.out.println("              [THICK SHAKES]     ");
						System.out.println("SrNo SHAKES                  RATE");
						System.out.println("1.   OREO                    15\n2.   CHOCOLATE               20\n3.   NUTELLA                 30\n4.   MANGO                   40\n5.   EXIT");
						System.out.println("ENTER UR CHOICE");
						x=sc.nextInt();
						System.out.println("");
						switch(x)
						{
						case 1:t1+=15;
							v1.addElement(new String("SHAKE=OREO")); 
							v2.addElement(new Integer(15));
							break;
						case 2:t1+=20;
							v1.addElement(new String("SHAKE=CHOCOLATE")); 
							v2.addElement(new Integer(20));
							break;
						case 3:t1+=30;
							v1.addElement(new String("SHAKE=NUTELLA"));
							v2.addElement(new Integer(30));
							break;
						case 4:t1+=40;
							v1.addElement(new String("SHAKE=MANGO"));
							v2.addElement(new Integer(40));
							break;
						case 5:System.out.println("SHAKE=EXICTED");
						System.out.println("");
							break;
						default:System.out.println("SORRY INVALID CHOICE...");
					   }
						if(x==1||x==2||x==3||x==4)
						{
							 y=0;
							 while(y!=1&&y!=2&&y!=3)
							 {	
						System.out.println("WHAT WILL BE THE SIZE?");
						System.out.println("                 [SIZE]          ");
						System.out.println("SrNo SIZE                     RATE");
						System.out.println("1.   SMALL                    5\n2.   MEDIUM                   10\n3.   LARGE                    15");
						System.out.println("ENTER UR CHOICE:");
						y=sc.nextInt();
						System.out.println("");
				     switch(y)
					{
					case 1:t1+=5;
					 	v1.addElement(new String ("SIZE=SMALL"));
					 	v2.addElement(new Integer(5));
						break;
					case 2:t1+=10;
					 	v1.addElement(new String ("SIZE=MEDIUM"));
					 	v2.addElement(new Integer(10));
						break;
					case 3:t1+=15;
					 	v1.addElement(new String ("SIZE=LARGE"));
					 	v2.addElement(new Integer(15));
						break;
					default:System.out.println("SORRY INVALID CHOICE...");
					System.out.println("PLZZ ENTER THE OTHER OPTIONS FOR SIZE");
					System.out.println("U CAN SELECT THE OPTIONS FROM 1,2&3");
						}
				   }
								}
						}
							break;
						case 4:t1+=80;
						v1.addElement(new String ("COLD COFFEE"));
						 o=0;
						 while(o!=1&&o!=2&&o!=3)
						 {
						System.out.println("WHAT WILL BE THE SIZE?");
						System.out.println("                 [SIZE]    			  ");
						System.out.println("SrNo SIZE                      RATE");
						System.out.println("1.   SMALL                     5\n2.   MEDIUM                    10\n3.   LARGE                    15");
						System.out.println("ENTER UR CHOICE:");
						o=sc.nextInt();
						System.out.println("");
					switch(o)
					{
					case 1:t1+=5;
						v1.addElement(new String ("SIZE=SMALL"));
						v2.addElement(new Integer(5));
						break;
					case 2:t1+=10;
						v1.addElement(new String ("SIZE=MEDIUM"));
						v2.addElement(new Integer(10));
						break;
					case 3:t1+=15;
						v1.addElement(new String ("SIZE=LARGE"));
						v2.addElement(new Integer(15));
						break;
					default:System.out.println("SORRY INVALID CHOICE...");
					System.out.println("PLZZ ENTER THE OTHER OPTIONS FOR SIZE");
					System.out.println("U CAN SELECT THE OPTIONS FROM 1,2&3");
				}
				   }
						 	break;
						case 5:System.out.println("EXITED");
						       System.out.println("");
							break;
						default:System.out.println("SORRY INVALID CHOICE...");
					   }
					  }
				}  
				}
				  	break;
				case 3:
					if(t1>300)
					{
						System.out.println("CONGRATES U HAVE WON OUR SPECIAL OFFER...");
						System.out.println("U WILL GET A DISCONT OF 50%");
						System.out.println("HERE IS UR BILL");
				    	System.out.println("*************************************RECEIPT***************************************");
					    System.out.println("");                						  
                        System.out.println("Enter ur mobile number:");
                        s1=sc.next(); 
                        System.out.println("--------------------------------------------------------------");
                        System.out.println("NAME                                                     PRIZE");
                        System.out.println("--------------------------------------------------------------");
                        for(z=0;z<v1.size();z++)
				       {
				    	 System.out.printf("%-20s                                      %s\n",v1.get(z).toString(),v2.get(z).toString());
				       }
                       System.out.println("--------------------------------------------------------------");
                       System.out.printf("%-20s                                      %s\n","TOTAL",t1);
                       System.out.println("--------------------------------------------------------------");
                       a1=t1*(0.5f);
                       System.out.println("UR FINAL AMOUNT AFTER DISCOUNT IS:"+(t1-a1));
					}
					else if(t1>0)
					{
					  System.out.println("Your total amount:  " +t1);
					  System.out.println("ENTER THE  MODE OF PAYMENT ");
					  System.out.println("1.CASH\n2.CARD\n3.PAYTM\n4.TAKEWAY\n5.COUPON");
				       p=sc.nextInt();   
					switch(p)
					{
					case 1:System.out.println("*************************************RECEIPT***************************************");
					       System.out.println("");
                           System.out.println("Mode:Cash");						  
                           System.out.print("Name:"+name);
                           System.out.println();
                           System.out.println("Enter ur mobile number:");
                           s1=sc.next(); 
                           System.out.println("--------------------------------------------------------------");
                           System.out.println("NAME                                                     PRIZE");
                           System.out.println("--------------------------------------------------------------");
                           for(z=0;z<v1.size();z++)
					       {
					    	 System.out.printf("%-20s                                      %s\n",v1.get(z).toString(),v2.get(z).toString());
					       }
                           System.out.println("--------------------------------------------------------------");
                             System.out.printf("%-20s                                      %s\n","TOTAL",t1);
                             System.out.println("--------------------------------------------------------------");
                             break;
					case 2:System.out.println("*************************************RECEIPT***************************************");
				           System.out.println("");
                           System.out.println("Mode:CARD");
                           System.out.println("Name:"+name);
                           System.out.println();
					       System.out.println("Enter ur mobile no:");
					       s1=sc.next();   
						   System.out.println("Enter the pin:");
						   s2=sc.next();
						   System.out.println("--------------------------------------------------------------");
						   System.out.println("NAME                                                     PRIZE");
					       System.out.println("--------------------------------------------------------------");
					       for(z=0;z<v1.size();z++)
					       {
					    	 System.out.printf("%-20s                                      %s\n",v1.get(z).toString(),v2.get(z).toString());
					       }
					       System.out.println("--------------------------------------------------------------");
					       System.out.printf("%-20s                                      %s\n","TOTAL",t1);
					       System.out.println("--------------------------------------------------------------");
						break;
					case 3:System.out.println("Mode:PAYTM");
					       System.out.print("Name:"+name);
					       System.out.println();
					       System.out.println("Enter ur mobile no:");
					       s1=sc.next();   						  
						   System.out.println("--------------------------------------------------------------");
						   System.out.println("NAME                                                     PRIZE");
					       System.out.println("--------------------------------------------------------------");
					       for(z=0;z<v1.size();z++)
					       {
					    	 System.out.printf("%-20s                                      %s\n",v1.get(z).toString(),v2.get(z).toString());
					       }
					       System.out.println("--------------------------------------------------------------");
					       System.out.printf("%-20s                                      %s\n","TOTAL",t1);
					       System.out.println("--------------------------------------------------------------");
						   System.out.println("SCAN THE BARCODE OR ELSE PAYTM ON 8454982994");
						break;
					case 4:System.out.println(name+" "+"UR PARCEL IS READY AND HERE IS UR BILL");
						   System.out.println("*************************************RECEIPT***************************************");
				           System.out.println(""); 
						   System.out.println("Mode:TAKEAWAY");						   
		                   System.out.println("Enter ur mobile number:");
		                   s1=sc.next(); 
		                   System.out.println("--------------------------------------------------------------");
		                   System.out.println("NAME                                                     PRIZE");
		                   System.out.println("--------------------------------------------------------------");
		                   for(z=0;z<v1.size();z++)
						       {
						    	 System.out.printf("%-20s                                      %s\n",v1.get(z).toString(),v2.get(z).toString());
						       }
		                   System.out.println("--------------------------------------------------------------");
		                   System.out.printf("%-20s                                      %s\n","TOTAL",t1);
		                   System.out.println("--------------------------------------------------------------");
						break;
					case 5:System.out.println("Enter the coupon code:");
					       s2=sc.next();
					       if(name.equals(s2))
					       {
					    	System.out.println("CONGRATES!!!!! UR COUPON CODE IS VALID......");  
					    	System.out.println("WILL GIVE U A DISCOUNT OF 40%");
					    	System.out.println("HERE IS UR BILL");
					    	System.out.println("*************************************RECEIPT***************************************");
						    System.out.println("");
	                        System.out.println("Mode:Cash");						  
	                        System.out.println("Enter ur mobile number:");
	                        s1=sc.next(); 
	                        System.out.println("--------------------------------------------------------------");
	                        System.out.println("NAME                                                     PRIZE");
	                        System.out.println("--------------------------------------------------------------");
	                        for(z=0;z<v1.size();z++)
					       {
					    	 System.out.printf("%-20s                                      %s\n",v1.get(z).toString(),v2.get(z).toString());
					       }
	                       System.out.println("--------------------------------------------------------------");
                           System.out.printf("%-20s                                      %s\n","TOTAL",t1);
                           System.out.println("--------------------------------------------------------------");
                           a1=t1*(0.4f);
                           System.out.println("UR FINAL AMOUNT AFTER DISCOUNT IS:"+(t1-a1));
					       }
						break;
						default:System.out.println("SORRY INVALID CHOICE...");
					}
				}
				   	System.out.println("                  THANK U SO MUCH FOR COMING"+" "+name+"!!!");
					System.out.println("                  HAVE A NICE DAY!!!");
						break;
				default:System.out.println("SORRY INVALID CHOICE...");
					}
				}	
			}
}
