# Summative-Assessment-3-

	#include <iostream>
	#include <string>
	#include <array>
	#include <math.h>
	using namespace std;

	void paymentcoffee(int coffeetea)
	{
		cout << "\n=====================================" << endl;
		cout << "\nThe total price is " << coffeetea << " AED" << endl;
		cout << "\nAmount Paid: ";
		double pay;
		cin >> pay;

		while (cin.fail() || pay < 1 || pay < coffeetea)
		{
			cout << "Error\n" << "Please try Again: ";
			cin.clear();
			cin.ignore(1000, '\n');
			cin >> pay;
		}

		double x = pay - coffeetea;
		cout << "\n=====================================" << endl;
		cout << "\nTOTAL AMOUNT" << endl;
		cout << "\nCash       " << pay << " AED " << endl;
		cout << "Change     " << x << " AED." << endl;
		cout << "\n-------------------------------------" << endl;
		cout << "\n\nThank you for ordering have a nice day!\n\n\n" << endl;
	}

	void coffee()
	{
		cout << "\n=====================================" << endl;
		cout << "\n           STARBOX MENU " << endl;
		cout << "\n=====================================" << endl;
		cout << "\nCoffee                    Price" << endl; 
		cout << "------                    -----" << endl;
		string coffee[3] = { "\n(3) Ice Coffee            3 AED", "(2) Milk Coffee           2 AED", "(1) Black Coffee          1 AED" };
		for (auto coff : coffee) {
				cout << coff << endl;
		}
		cout << "\n=====================================" << endl;
		cout << endl;

		cout << "Please select the type of coffee \n" << "that you would like to purchase." << endl;
		cout << "\nInsert their corresponding number." << endl;
		cout << "eg. = 3 for Ice coffee" << endl;
		cout << "\nEnter Choice: ";
		int coffeetea;
		cin >> coffeetea;

		while (cin.fail() || coffeetea != 3 && coffeetea != 2 && coffeetea != 1)
		{
			cout << "Invalid Input\n" << "Please try Again: ";
			cin.clear();
			cin.ignore(1000, '\n');
			cin >> coffeetea;
		}

		if (coffeetea == 3 )
		{
			cout << "\nIce coffee coming right up!\n";
		}
		else if (coffeetea == 2)
		{
			cout << "\nMilk coffee coming right up!\n";
		}
		else
		{
		cout << "\nBlack coffee coming right up!";
	    }

		char sugar;

		do {
			cout << "\n=====================================" << endl;
			cout << "\nDo you want sugar? (Y/N)" << endl;
			cout << "\nEnter Choice: ";
			cin >> sugar;
		} while ((sugar != 'Y') && (sugar != 'y') && (sugar != 'N') && (sugar != 'n'));

		switch (sugar)
		{
		case 'Y':
		case 'y':
			cout << "\n~ Sugar is being added ~" << endl;
			break;
		case 'N':
		case 'n':
			cout << "\n~ Sugar will not be added ~" << endl;
			break;

		default:
			cout << "\nInvalid Input" << endl;
			break;
		}
		paymentcoffee(coffeetea);
	}

	void paymenttea(int coffeetea)
	{
		cout << "\n=====================================" << endl;
		cout << "\nThe total price is " << coffeetea << " AED" << endl;
		cout << "\nAmount: ";
		double pay;
		cin >> pay;

		while (cin.fail() || pay < 1 || pay < coffeetea)
		{
			cout << "Error\n" << "Please try Again: ";
			cin.clear();
			cin.ignore(1000, '\n');
			cin >> pay;
		}

		double x = pay - coffeetea;
		cout << "\n=====================================" << endl;
		cout << "\nTOTAL AMOUNT" << endl;
		cout << "\nCash       " << pay << " AED " << endl;
		cout << "Change     " << x << " AED." << endl;
		cout << "\n-------------------------------------" << endl;
		cout << "\n\nThank you for ordering have a nice day!\n\n\n" << endl;
	}

	void tea()
	{
		cout << "\n=====================================" << endl;
		cout << "\n           STARBOX MENU " << endl;
		cout << "\n=====================================" << endl;
		cout << "\Tea                    Price" << endl;
		cout << " ----                   -----" << endl;
		string Teaa[3] = { "\n(3) Ice Tea            3 AED", "(2) Milk Tea           2 AED", "(1) Black Tea          1 AED" };
		for (auto tea : Teaa) {
			cout << tea << endl;
		}
		cout << "\n=====================================" << endl;
		cout << endl;

		cout << "Please select the type of tea \n" << "that you would like to purchase." << endl;
		cout << "\nInsert their corresponding number." << endl;
		cout << "eg. = 3 for Ice Tea" << endl;
		cout << "\nEnter Choice: ";
		int coffeetea;
		cin >> coffeetea;

		while (cin.fail() || coffeetea != 3 && coffeetea != 2 && coffeetea != 1)
		{
			cout << "Invalid Input\n" << "Please try Again: ";
			cin.clear();
			cin.ignore(1000, '\n');
			cin >> coffeetea;
		}

		if (coffeetea == 3)
		{
			cout << "\nIce Tea coming right up!\n";
		}
		else if (coffeetea == 2)
		{
			cout << "\nMilk Tea coming right up!\n";
		}
		else
		{
			cout << "\nBlack Tea coming right up!";
		}

		char sugar;

		do {
			cout << "\n=====================================" << endl;
			cout << "Do you want sugar? (Y/N)" << endl;
			cout << "\nEnter Choice: ";
			cin >> sugar;
		} while ((sugar != 'Y') && (sugar != 'y') && (sugar != 'N') && (sugar != 'n'));

		switch (sugar)
		{
		case 'Y':
		case 'y':
			cout << "\n~ Sugar is being added ~" << endl;
			break;
		case 'N':
		case 'n':
			cout << "\n~ Sugar will not be added ~" << endl;
			break;

		default:
			cout << "\nInvalid Input" << endl;
			break;
		}
		paymenttea(coffeetea);
	}

	int main()
	{
		cout << "\n====================================================================" << endl;
		cout << "\n                  |||||||||||||" << endl;
		cout << "Hello! Welcome to || StarBox || What would you like, Coffee or Tea? " << endl; 
		cout << "                  |||||||||||||" << endl;
		cout << "\n====================================================================" << endl;
		cout << "\nC for coffee\n" << "T for Tea\n";
		string answer;
		cout << "\nEnter Choice: " ;
		cin >> answer;

		while (cin.fail() || answer != "C" && answer != "c" && answer != "T" && answer != "t")
		{
			cout << "Invalid Input\n"<< "Please try Again: ";
			cin.clear();
			cin.ignore(1000, '\n');
			cin >> answer;
		}

		if (answer == "C" || answer == "c") 
		{
			coffee();
		}
		else 
		{
			tea();
		}
		return 0;

	}



















