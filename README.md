# HOTEL-MANAGEMENT-SYSTEM
Quantity present in hotel ,total sell,total collection,remaining items in hotel
//PROJECT ON HOTEL MANAGEMENT SYSTEM
/*
This project will be hotel management project in which we have the information of the item and room that we have in the hotel,
and what are the food items ordered by the customer ,also we have the information how many rooms are alloted to them.
And also this project tells us the sells and the remaining food stock we have and total collection of the day.

*/  
#include<iostream>
using namespace std;

int main(){
	int quant;
	int choice;
	
	//food items that hold the quantity of food items in the hotel.
	
	int Qrooms=0 , Qpasta=0, Qburger=0, Qnoodles=0, Qshake=0, Qbiryani=0;  //Qpasta is the no. of pasta that we have in the hotel   ansd so on.
	
	 // items that we have sold in the hotel
	int Srooms=0, Spasta=0 ,Sburger=0, Snoodles=0, Sshake=0,Sbiryani=0;
	//now the total price of each of the items
	int Total_rooms=0, Total_pasta=0,Total_burger=0,Total_noodles=0,Total_shake=0,Total_biryani=0; 
	
	cout<<"\n\t Quantity of items we have"  ;
	cout<<"\n Rooms available:";
	cin>>Qrooms;
	cout<<"\n Quantity of pasta :";
	cin>>Qpasta;	
	cout<<"\n Quantity of burger :";
	cin>>Qburger;
	cout<<"\n Quantity of noodles :";
	cin>>Qnoodles;
	cout<<"\n Quantity of shake :";
	cin>>Qshake ;
	cout<<"\n Quantity of biryani ";
	cin>>Qbiryani;
		
	m:
	cout<<"\n\t\t\t please select from the menu options ";
	cout<<"\n\n1) Rooms ";
	cout<<"\n2) Pasta ";
	cout<<"\n3) Burger" ; 
	cout<<"\n4) Noodles" ;
	cout<<"\n5) Shake " ;
	cout<<"\n6) Biryani" ;
	cout<<"\n7) Information regarding sales and collection";
	cout<<"\n8) Exit";
	
	
	cout<<"\n\n Please Enter your choice!";
	cin>>choice;
	
	switch(choice)
{
	case 1:
		cout<<"\n\n Enter the number of rooms you want :";
		cin>>quant;
		if(Qrooms-Srooms>=quant){
			Srooms=Srooms+quant;
			Total_rooms=Total_rooms+quant*1500 ; //total price of the room
			cout<<"\n\n\t\t"<<quant<<"rooms/rooms have been alloted to you!";
		}
		else
		cout<<"\n\tOnly"<<Qrooms-Srooms<<"Rooms remaining in hotel ";
		break;
		
		case 2:
		cout<<"\n\n Enter the quantity of pasta :";
		cin>>quant;
		if(Qpasta-Spasta>=quant){
			Spasta=Spasta+quant;
			Total_pasta=Total_pasta+quant*250 ;//price of a pasta=250
			cout<<"\n\n\t\t"<<quant<<"pasta is the order!";
		}
		else
		cout<<"\n\tOnly"<<Qpasta-Spasta<<"pasata remaining in hotel ";
		break;
		
		case 3:
		cout<<"\n\n Enter the quantity of burger :";
		cin>>quant;
		if(Qburger-Sburger>=quant){
			Sburger=Sburger+quant;
			Total_burger=Total_burger+quant*200 ;//price of a burger=200
			cout<<"\n\n\t\t"<<quant<<"burger is the order!";
		}
		else
		cout<<"\n\tOnly"<<Qburger-Sburger<<"burger remaining in hotel ";
		break;
		
		
	case 4:
		cout<<"\n\n Enter the quantity of noodle :";
		cin>>quant;
		if(Qnoodles-Snoodles>=quant){
			Snoodles=Snoodles+quant;
			Total_noodles=Total_noodles+quant*150 ;//price of a noodle=150
			cout<<"\n\n\t\t"<<quant<<"noodle is the order!";
		}
		else
		cout<<"\n\tOnly"<<Qnoodles-Snoodles<<"noodle remaining in hotel ";
		break;
		
			case 5:
		cout<<"\n\n Enter the quantity of shake :";
		cin>>quant;
		if(Qshake-Sshake>=quant){
			Sshake=Sshake+quant;
			Total_shake=Total_shake+quant*150 ;//price of a noodle=150
			cout<<"\n\n\t\t"<<quant<<"shake is the order!";
		}
		else
		cout<<"\n\tOnly"<<Qshake-Sshake<<"shake remaining in hotel ";
		break;
		
			case 6:
		cout<<"\n\n Enter the quantity of biryani :";
		cin>>quant;
		if(Qbiryani-Sbiryani>=quant){
			Sbiryani=Sbiryani+quant;
			Total_biryani=Total_biryani+quant*150 ;//price of a noodle=150
			cout<<"\n\n\t\t"<<quant<<"biryani is the order!";
		}
		else
		cout<<"\n\tOnly"<<Qbiryani-Sbiryani<<"biryani remaining in hotel ";
		break;
	
	case 7:
	cout<<"\n\t Details of the sells collection ";
	cout<<"\n\n Number of rooms we had : "<<Qrooms;
	cout<<"\n\n Number of rooms we gave for rent "<<Srooms ;
	cout<<"\n\n Remaining rooms : "<<Qrooms-Srooms;
	cout<<"\n\n Total rooms collection for the day : "<<Total_rooms;
	

	cout<<"\n\n Number of pasta we had : "<<Qpasta;
	cout<<"\n\n Number of pasta we sold "<<Spasta ;
	cout<<"\n\n Remaining pastas : "<<Qpasta-Spasta;
	cout<<"\n\n Total pasta collection for the day : "<<Total_pasta;


	cout<<"\n\n Number of burger we had : "<<Qburger;
	cout<<"\n\n Number of burger we sold "<<Sburger ;
	cout<<"\n\n Remaining burger : "<<Qburger-Sburger;
	cout<<"\n\n Total burger collection for the day : "<<Total_burger;
	
	
	cout<<"\n\n Number of Noodles we had : "<<Qnoodles;
	cout<<"\n\n Number of Noodles we sold "<<Snoodles ;
	cout<<"\n\n Remaining Noodles : "<<Qnoodles-Snoodles;
	cout<<"\n\n Total Noodles collection for the day : "<<Total_noodles;
	
	
	cout<<"\n\n Number of Biryani we had : "<<Qbiryani;
	cout<<"\n\n Number of Biryani we sold "<<Sbiryani ;
	cout<<"\n\n Remaining Biryani : "<<Qbiryani-Sbiryani;
	cout<<"\n\n Total Biryani collection for the day : "<<Total_biryani;
	
	case 8:
		exit(0);
		
		default:
			cout<<"\n Please select the numbers mentioned above !";

	
	}	
	
	goto m;
	
	
}
