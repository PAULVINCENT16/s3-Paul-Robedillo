# s3-Paul-Robedillo
#include <iostream>
#include <string>
#include <math.h>
#include <array>

using namespace std;

int main()
{
	int pickings{};
	string menu[4][4] = {
		{"Coffee\t\t", "Price(AED)\t", "Tea(AED)\t", "Price\t"},
		{"Iced Coffee\t", "3(AED)\t\t", "Iced Tea\t", "3(AED)\t"},
		{"Milk Coffee\t", "2(AED)\t\t", "Milk Tea\t", "2(AED)\t"},
		{"Black Coffee\t", "1(AED)\t\t", "Black Tea\t", "1(AED)\t"}
	};

	for (int i = 0; i < 4; i++) {
		for (int j = 0; j < 4; j++) {
			cout << menu[i][j] << " ";
		}
		cout << endl;
	}

	char drink;
	cout << "Pick a drink you like and press 'C' Coffee or 'T' Tea?" << endl;
	cin >> drink;
	while (cin.fail()) {
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Invalid input.\nPlease enter a valid option:";
		cin >> drink;
	}
	



	if (drink == 'C' || drink == 'c') {
		cout << "What Coffee would you like to drink?" << endl;
		cout << "1. Iced Coffee" << endl;
		cout << "2. Milk Coffee" << endl;
		cout << "3. Black Coffee" << endl;
		cin >> pickings;
		while (cin.fail()) {
		    cin.clear();
		    cin.ignore(1000, '\n');
		    cout << "Invalid input.\nPlease enter a valid option:";
		    cin >> pickings;
		    
		}
	    
	}
	else if (drink == 'T' || drink == 't') {
		cout << "What Tea would you like to drink?" << endl;
		cout << "1. Iced Tea" << endl;
		cout << "2. Milk Tea" << endl;
		cout << "3. Black Tea" << endl;
		cin >> pickings;
		while (cin.fail()) {
		    cin.clear();
		    cin.ignore(1000, '\n');
		    cout << "Invalid input.\nPlease enter a valid option:";
	    	cin >> pickings;
		    
		}

	}
	else {
		
		cin >> pickings;
		while (cin.fail()) {
	    	cin.clear();
		    cin.ignore(1000, '\n');
		    cout << "Invalid input.\nPlease enter a valid option:";
		    cin >> pickings;
		    
		}
	}

	double money;
	char sweets;
	cout << "You want it with sugar? press 'Y' if you want and 'N' if you dont: " << endl;
	cin >> sweets;
	while (cin.fail()) {
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Invalid input.\nPlease enter a valid option:";
		cin >> sweets;
	    
	}


	switch (pickings) {
	case 1:
		cout << "Processing." << endl;
		if (sweets == 'Y' || sweets == 'y') {
			cout << "Okay i will put Sugar. " << endl;
			cout << "And the total price of your order." << endl;
			cout << "It was 3.15(AED) with 5% vat for the receipt." << endl;
			cout << "How much your money?";
			cin >> money;
			cout << "Your change is: " << money - 3.15;
			cout << "\tEnjoy your drink." << endl;

			    
			
	

		}
		else if (sweets == 'N' || sweets == 'n') {
			cout << "Okay i won't put Sugar. " << endl;
			cout << "And the total price of your order." << endl;
			cout << "It was 3.15(AED) with 5% vat for the receipt." << endl;
			cout << "How much your money?";
			cin >> money;
			cout << "Your change is: " << money - 3.15;
			cout << "\tEnjoy your drink." << endl;
			
		}
		else {
			
			cin >> pickings;
			while (cin.fail()) {
	        	cin.clear();
	        	cin.ignore(1000, '\n');
	        	cout << "Invalid input.\nPlease enter a valid option:";
	        	cin >> pickings;
		}
		    
		}
		break;
		

	case 2:
		cout << "Processing." << endl;
		if (sweets == 'Y' || sweets == 'y') {
			cout << "Okay i will put Sugar. " << endl;
			cout << "And the total price of your order." << endl;
			cout << "It was 2.10(AED) with 5% vat for the receipt." << endl;
			cout << "How much your money?";
			cin >> money;
			cout << "Your change is: " << money - 2.10;
			cout << "\tEnjoy your drink." << endl;

			    
			
			

		}
		else if (sweets == 'N' || sweets == 'n') {
			cout << "Okay i won't put Sugar. " << endl;
			cout << "And the total price of your order." << endl;
			cout << "It was 2.10(AED) with 5% vat for the receipt." << endl;
			cout << "How much your money?";
			cin >> money;
			cout << "Your change is: " << money - 2.10;
			cout << "\tEnjoy your drink." << endl;

			    
			
			
		}
		else {

			cin >> pickings;
			while (cin.fail()) {
	        	cin.clear();
	        	cin.ignore(1000, '\n');
	        	cout << "Invalid input.\nPlease enter a valid option:";
	        	cin >> pickings;
			    
			}
			
		}
		break;

	case 3:
		cout << "Processing." << endl;
		if (sweets == 'Y' || sweets == 'y') {
			cout << "Okay i will put Sugar. " << endl;
			cout << "And the total price of your order." << endl;
			cout << "It was 1.05(AED) with 5% vat for the receipt." << endl;
			cout << "How much your money?";
			cin >> money;
			cout << "Your change is: " << money - 1.05;
			cout << "\tEnjoy your drink." << endl;

			    
			
			
			
		}
		else if (sweets == 'N' || sweets == 'n') {
			cout << "Okay i won't put Sugar. " << endl;
			cout << "And the total price of your order." << endl;
			cout << "It was 1.05(AED) with 5% vat for the receipt." << endl;
			cout << "How much your money?";
			cin >> money;
			cout << "Your change is: " << money - 1.05;
			cout << "\tEnjoy your drink." << endl;
			    
		
			
		}
		else {
			cin >> pickings;
			while (cin.fail()) {
	    	cin.clear();
	       	cin.ignore(1000, '\n');
	       	cout << "Invalid input.\nPlease enter a valid option:";
	    	cin >> pickings;
			    
			}
		

			    
			
		}
		break;

	default:
		cout << "Invalid input." << endl;
		cin >> pickings;
		while (cin.fail()) {
	    	cin.clear();
	       	cin.ignore(1000, '\n');
	       	cout << "Invalid input.\nPlease enter a valid option:";
	    	cin >> pickings;
		    
		}
		break;
	    
	}
    
}
