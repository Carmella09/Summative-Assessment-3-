# Summative-Assessment-3-

#include <iostream>
#include <string>
using namespace std;
int main()
{
	cout << "\n";
	cout << "Coffee               Price(AED)     |       Tea               Price(AED)" << endl; 
	cout << "(I) Ice Coffee            3         |       (I) Ice Tea                     " << endl;
	cout << "(M) Milk Coffee           2         |       (M) Milk Tea                    " << endl;
	cout << "(B) Black Coffee          1         |       (B) Black Tea                   " << endl;

	string answer;
	cout << "\nHello! What would you like, Coffee or Tea? "; 
	cin >> answer;

	while (cin.fail())
	{
		cout << "\nInvalid Input. Please enter your answer again: " << endl;
		cin.clear();
		cin.ignore(1000, '\n');
		cin >> answer;
	}

	while (answer == "Coffee" || answer == "coffee")
	{
		cout << "\nPlease choose from the menu above which Coffee would you like." << endl;
		cout << "Insert their coresponding letter." << endl;
		cout << "eg. = I for Ice coffee\n" << endl;
		string coffeetea;
		cin >> coffeetea;

		if (coffeetea == "I" || coffeetea == "i")
		{
			cout << "\nYou have chosen Ice coffee." << endl;
		}
		else if (coffeetea == "M" || coffeetea == "m")
		{
			cout << "\nYou have chosen Milk coffee." << endl;
		}
		else if (coffeetea == "B" || coffeetea == "b")
		{
			cout << "\nYou have chosen BLack coffee." << endl;
		}
		else
		{
			cout << "\nInvalid Input. Please enter your answer again: " << endl;
			cin.clear();
			cin.ignore(1000, '\n');
			cin >> coffeetea;
		}

		cout << "\nDo you want to add suger? (Y/N)" << endl;
		char sugar;
		cin >> sugar;

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
			cout << "\nInvalid Input. Please enter your answer again: " << endl;
			cin.clear();
			cin.ignore(1000, '\n');
			cin >> sugar;
		}

	}

	while (answer == "Tea" || answer == "tea")
	{
		cout << "Please choose from the menu above which Tea would you like" << endl;
		cout << "\nDo you want to add suger? (Y/N)" << endl;
		char sugar;
		cin >> sugar;

		cout << "\nPlease choose from the menu above which Coffee would you like." << endl;
		cout << "Insert their coresponding letter." << endl;
		cout << "eg. = I for Ice coffee\n" << endl;
		string coffeetea;
		cin >> coffeetea;

		if (coffeetea == "I" || coffeetea == "i")
		{
			cout << "\nYou have chosen Ice coffee." << endl;
		}
		else if (coffeetea == "M" || coffeetea == "m")
		{
			cout << "\nYou have chosen Milk coffee." << endl;
		}
		else if (coffeetea == "B" || coffeetea == "b")
		{
			cout << "\nYou have chosen BLack coffee." << endl;
		}
		else
		{
			cout << "\nInvalid Input. Please enter your answer again: " << endl;
			cin.clear();
			cin.ignore(1000, '\n');
			cin >> coffeetea;
		}

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
			cout << "\nInvalid Input. Please enter your answer again: " << endl;
			cin.clear();
			cin.ignore(1000, '\n');
			cin >> sugar;
		}

	}
	
	cout << "your payment will be ";
}



















