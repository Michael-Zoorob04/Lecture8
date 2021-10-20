DAYS IN A MONTH

#include <iostream>

using namespace std;

int main()
{
    int daysmonth;

    cout << "Please enter a month number [1-12]: " << "\n";
    cin >> daysmonth;

    switch (daysmonth)
    {
    case 1: cout << "31 days in January.";
        break;
    case 2: cout << "28 or 29 days in February.";
        break;
    case 3: cout << "31 days in March.";
        break;
    case 4: cout << "30 days in April.";
        break;
    case 5: cout << "31 days in May.";
        break;
    case 6: cout << "30 days in June.";
        break;
    case 7: cout << "31 days in July.";
        break;
    case 8: cout << "31 days in August.";
        break;
    case 9: cout << "30 days in September.";
        break;
    case 10: cout << "31 days in October.";
        break;
    case 11: cout << "30 days in November.";
        break;
    case 12: cout << "31 days in December.";
        break;
    default: cout << "Wrong input! Try again.";

    }
    return 0;

}
===========================================================
FUEL ME UP
  
  #include<iostream>

using namespace std;

int main()
      {

	char fueltype;
      cout << "Please enter the type of fuel you want: \n";
	    cin >> fueltype;

	int litres;
	  cout << "Number of litres: \n";
	    cin >> litres;

	char c = toupper(fueltype);
	   if (litres > 1)
	  {


		switch (c) {
		   case 'P':

			   cout << "The price is: " << litres * 2.44 << "\n"; 
			break;

		case 'D': 
			
			   cout << "The price is: " << litres * 2.38 << "\n"; 
			break;

		default:

			cout << "That is an invalid fuel type! Please try again.\n";
		}


	}

} 
======================================================================
TEMPERATURE
  
  #include<iostream>

using namespace std;

int main()
{
    float F, C;
    int choice;

    cout << "Choose option 1 or 2:" << "\n";
    cout << "1 for celsius to fahrenheit." << "\n";
    cout << "2 for fahrenheit to celsius." << "\n";
    cin >> choice;


    switch (choice) {

    case 1:
        cout << "Please enter the temperature in celsius: ";
        cin >> C;

        F = (1.8 * C) + 32.0;
        cout << "\nThe temperature in farenheit is: " << F << " F";
        break;

    case 2:

        cout << "Please enter the temperature in fahrenheit: ";
        cin >> F;

        C = (F - 32) / 1.8;
        cout << "\nThe temperature in celsius is: " << C << " C";
        break;

    default:
        cout << "Incorrect input. Please try again.";

        return 0;
    }

}
  =======================================================================
  GRADE CHANGE


#include <iostream>
#include <string>


using namespace std;


int main() {

    cout << "Please enter your name: " << endl;
    string name;
    
    getline(cin, name);


    cout << "\nPlease enter your marks (0-100): ";

    
    int marks;

    cin >> marks;
    
    if (cin.fail())
    {
        cin.clear();
           cin.ignore();
        cout << "Invalid input. Please try again.\n: ";
    }
    else if (marks > 100)
    {
        cout << "\nKindly type in numbers within the range of 0-100.\n";
    }

    else


    switch (marks / 10) {

    case 10:
       case 9:
    case 8:
    {
        cout << name << " got an A.";
        break;
    }
    case 7:
    {
        cout << name << " got a B.";
        break;
    }
    case 6:
    {
        cout << name << " got a C.";
        break;
    }
    case 5:
    {
        cout << name << " got a D.";
        break;
    }
    case 4:
    {
        cout << name << " got an E.";
        break;
    }
    default:
    {
        cout << name << " got an F.\n";
    }
    }

}
  
