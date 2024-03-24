//
// Created by Amirjon Alijonov FED2 230298
//
#include <iostream>
#include <cmath>
#include <cstdlib>
#include <ctime>

using namespace std;

int main() {
    cout << "PROBLEM 1\n";
    int x = 0;
    cin >> x;
    if (x>0) {
       cout << "Positive" << endl << endl;
    } else {
        cout << "Negative" << endl << endl;
    }

    cout << "PROBLEM 2\n";
    if (x>0) {
        cout << "The number is positive ";
        if (x % 2 == 0) {
            cout << "and even" << endl << endl;
        } else {
            cout << "and odd" << endl << endl;
        }
    } else {
        cout << "The number is negative ";
        if (x % 2 == 0) {
            cout << "and even" << endl << endl;
        } else {
            cout << "and odd" << endl << endl;
        }
    }

    cout << "PROBLEM 3\n";
    int a3=0,b3=0,c3=0;
    cin >> a3 >> b3 >> c3;
    if (a3 > b3 && a3 > c3) {
        cout << a3 << " is the largest" << endl << endl;
    }

    else if (b3 > a3 && b3 > c3) {
        cout << b3 << " is the largest" << endl << endl;
    }

    else if (c3 > b3 && c3 > a3) {
        cout << c3 << " is the largest" << endl << endl;
    }

    cout << "PROBLEM 4\n";
    int a4 = 0, b4 = 0;
    cin >> a4 >> b4;
    if (a4 % b4 == 0) {
        cout << a4 << " is divisible by " << b4 << endl << endl;
    } else {
        cout << a4 << " is not divisible by " << b4 << endl << endl;
    }


    cout << "PROBLEM 5\n";
    int a5 = 0;
    cin >> a5;
    if ((a5 % 4 == 0 && a5 % 100 != 0) || (a5 % 400 == 0)) {
        cout << a5 << " is a leap year" << endl << endl;
    } else {
        cout << a5 << " is not a leap year" << endl << endl;
    }

    cout << "PROBLEM 6\n";
    double a6 = 0, b6 = 0, c6 = 0;
    cin >> a6 >> b6 >> c6;
    double discriminant = b6 * b6 - 4 * a6 * c6;

    if (discriminant > 0) {
        double root1 = (-b6 + sqrt(discriminant)) / (2 * a6);
        double root2 = (-b6 - sqrt(discriminant)) / (2 * a6);
        cout << "x1 = " << root1 << endl;
        cout << "x2 = " << root2 << endl << endl;
    } else {
        double root1 = -b6 / (2 * a6);
        cout << "x1 = " << root1 << endl;
        cout << "x2 = " << root1 << endl << endl;
    }

    cout << "PROBLEM 7\n";
    int a7 = 0, b7 = 0, c7 = 0;
    cin >> a7 >> b7 >> c7;
    if ((a7 + b7) > c7 || (a7 + c7) > b7 || (c7 + b7) > a7) {
        cout << "The triangle is valid" << endl << endl;
    } else {
        cout << "The triangle is not valid" << endl << endl;
    }

    cout << "PROBLEM 8\n";
    char a8;
    cin >> a8;
    if (islower(a8)) {
        cout << "Lowercase alphabet" << endl << endl;
    }
    else if (isupper(a8)) {
        cout << "Uppercase alphabet" << endl << endl;
    } else {
        cout << "It is not an alphabet" << endl << endl;
    }

    cout << "PROBLEM 9\n";
    int a9 = 0;
    cin >> a9;
    if (a9 < 20) {
        cout << "too slow" << endl << endl;
    } else if (a9 > 80) {
        cout << "too fast" << endl << endl;
    } else {
        cout << "just right" << endl << endl;
    }

    cout << "PROBLEM 10\n";
    double x10, y10;
    cin >> x10 >> y10;

    double distance = sqrt(x10 * x10 + y10 * y10);

    if (distance <= 10) {
        cout << "Point (" << x << "," << y10 << ") is in circle." << endl << endl;
    } else {
        cout << "Point (" << x << "," << y10 << ") is not in circle." << endl << endl;
    }

    cout << "PROBLEM 11\n";
    float w_1_11 = 0, p_1_11 = 0, w_2_11 = 0, p_2_11 = 0;
    cout << "Enter weight and price for package 1: ";
    cin >> w_1_11 >> p_1_11;
    cout << "Enter weight and price for package 2: ";
    cin >> w_2_11 >> p_2_11;

    float pack1 = w_1_11 / p_1_11;
    float pack2 = w_2_11 / p_2_11;

    if (pack1 > pack2) {
        cout << "Package 1 has a better price" << endl << endl;
    } else if (pack1 < pack2) {
        cout << "Package 2 has a better price" << endl << endl;
    } else {
        cout << "Two packages have the same price." << endl << endl;
    }

    cout << "PROBLEM 12\n";
    int number;
    cout << "Enter a three-digit integer: ";
    cin >> number;

    int originalNumber = number;
    int digit1 = number % 10;
    number /= 10;
    number /= 10;
    int digit3 = number;

    if (digit1 == digit3) {
        cout << originalNumber << " is a palindrome" << endl;
    } else {
        cout << originalNumber << " is not a palindrome" << endl;
    }


    cout << "PROBLEM 13\n";
    char a13;
    cin >> a13;
    switch(a13) {
        case 'g':
            cout << "Go!" << endl << endl;
            break;
        case 'y':
            cout << "Get ready!" << endl << endl;
            break;
        case 'r':
            cout << "Stop" << endl << endl;
            break;
        default:
            cout << "Invalid input" << endl << endl;
    }

    cout << "PROBLEM 14\n";
    int a14, b14;
    string daysOfWeek[] = {"Not zero please","Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"};
    cout << "Enter today's day: ";
    cin >> a14;
    cout << "Enter the number of days elapsed since today: ";
    cin >> b14;
    int futureDay = (a14+b14) % 7;
    cout << "Today is " << daysOfWeek[a14] << " and the future day is " << daysOfWeek[futureDay] << endl << endl;

    cout << "PROBLEM 15\n";
    int a15;
    cin >> a15;
    switch ((a15 <= 100 && a15 >= 90) ? 'A' : (a15 <= 89 && a15 >= 80) ? 'B' : (a15 <= 79 && a15 >= 70) ? 'C' : (a15 <= 69 && a15 >= 60) ? 'D' : (a15 <= 59 && a15 >= 0) ? 'F' : 0) {
        case 'A':
            cout << "A" << endl << endl;
            break;
        case 'B':
            cout << "B" << endl << endl;
            break;
        case 'C':
            cout << "C" << endl << endl;
            break;
        case 'D':
            cout << "D" << endl << endl;
            break;
        case 'F':
            cout << "F" << endl << endl;
            break;
        case 0:
            cout << "Invalid input" << endl << endl;
    }

    cout << "PROBLEM 16\n";
    int a16;
    cin >> a16;
    switch (a16 > 0 ? 1 : a16 < 0 ? -1 : 0) {
        case 1:
            cout << "Positive" << endl << endl;
            break;
        case -1:
            cout << "Negative" << endl << endl;
            break;
        case 0:
            cout << "It is zero" << endl << endl;
            break;
    }

    cout << "PROBLEM 17\n";
    char a17;
    cin >> a17;
    switch (a17) {
        case 'u':
            cout << "Salom" << endl << endl;
            break;
        case 'e':
            cout << "Hello" << endl << endl;
            break;
        case 'r':
            cout << "Привет" << endl << endl;
            break;
        case 'g':
            cout << "Hallo" << endl << endl;
            break;
        default:
            cout << "I do not know this language:(" << endl << endl;
    }

    cout << "PROBLEM 18\n";
    int a18;
    cin >> a18;

    // Program 1
    if (a18 > 0 && a18 <= 1) {
        cout << 3500 << endl << endl;
    } else if (a18 > 1 && a18 <= 3) {
        cout << 5500 << endl << endl;
    } else if (a18 > 3 && a18 <= 10) {
        cout << 8500 << endl << endl;
    } else if (a18 > 10 && a18 <= 20) {
        cout << 10500 << endl << endl;
    } else if (a18 > 20) {
        cout << "The package cannot be shipped." << endl << endl;
    } else {
        cout << "Invalid input." << endl << endl;
    }

    // Program 2
    switch ((a18 > 0 && a18 <= 1) ? 1 : (a18 > 1 && a18 <= 3) ? 2 : (a18 > 3 && a18 <= 10) ? 3 : (a18 > 10 && a18 <= 20) ? 4 : (a18 > 20) ? 5 : 0) {
        case 1:
            cout << 3500 << endl << endl;
            break;
        case 2:
            cout << 5500 << endl << endl;
            break;
        case 3:
            cout << 8500 << endl << endl;
            break;
        case 4:
            cout << 10500 << endl << endl;
            break;
        case 5:
            cout << "The package cannot be shipped." << endl << endl;
            break;
        case 0:
            cout << "Invalid input." << endl << endl;
    }

    cout << "PROBLEM 19\n";
    int a19;
    cin >> a19;

    switch (a19) {
        case 0:
            cout << "Zero" << endl;
            break;
        case 1:
            cout << "One" << endl;
            break;
        case 2:
            cout << "Two" << endl;
            break;
        case 3:
            cout << "Three" << endl;
            break;
        case 4:
            cout << "Four" << endl;
            break;
        case 5:
            cout << "Five" << endl;
            break;
        case 6:
            cout << "Six" << endl;
            break;
        case 7:
            cout << "Seven" << endl;
            break;
        case 8:
            cout << "Eight" << endl;
            break;
        case 9:
            cout << "Nine" << endl;
            break;
        default:
            cout << "It is not a digit" << endl;
    }

    cout << "PROBLEM 20\n";    int month;
    cin >> month;

    switch (month) {
        case 1:
            cout << "In January there is a new year" << endl;
            break;
        case 2:
            cout << "In February there are no holidays." << endl;
            break;
        case 3:
            cout << "In March there is:\n"
                 << "- International Women’s Day, 8 March\n"
                 << "- Navruz, 21 March" << endl;
            break;
        case 4:
            cout << "In April there are no holidays." << endl << endl;
            break;
        case 5:
            cout << "In May there are no holidays." << endl << endl;
            break;
        case 6:
            cout << "In February, April,\n"
                    "June, July, August, November\n"
                    "there is no holidays. There\n"
                    "are Ramadan Hayit and Kurban\n"
                    "Hayit but their dates change." << endl << endl;
            break;
        case 7:
            cout << "In July there are no holidays." << endl << endl;
            break;
        case 8:
            cout << "In August there are no holidays." << endl << endl;
            break;
        case 9:
            cout << "In September there are no holidays." << endl << endl;
            break;
        case 10:
            cout << "In October there is teachers' day" << endl << endl;
            break;
        case 11:
            cout << "In November there are no holidays." << endl << endl;
            break;
        case 12:
            cout << "In December there a New Year" << endl << endl;
            break;
        default:
            cout << "Invalid input! Please enter a month number between 1 and 12." << endl;
    }

    cout << "PROBLEM 21\n";
    srand(time(0));
    int a21;
    cout << "There will be odd or even number?\nYour stake: (1 for odd, 0 for even): ";
    cin >> a21;
    int random_value = rand() % 51;
    cout << random_value << endl;
    if ((random_value % 2 == 0) && a21 == 0) {
        cout << "You won! The random number is an even number." << endl << endl;
    } else if (random_value % 2 == 1 && a21 == 1) {
        cout << "You won! The random number is an odd number." << endl << endl;
    } else {
        cout << "Next time you will win babe." << endl << endl;
    }

    cout << "PROBLEM 22\n";
    srand(time(0));

    // Generate a random rank and suit index
    int rankIndex = rand() % 13;
    int suitIndex = rand() % 4;

    // Output the randomly picked card
    cout << "The card you picked is the ";
    if (rankIndex == 0) {
        cout << "Ace";
    } else if (rankIndex >= 1 && rankIndex <= 9) {
        cout << rankIndex + 1;
    } else {
        switch (rankIndex) {
            case 10:
                cout << "Jack";
                break;
            case 11:
                cout << "Queen";
                break;
            case 12:
                cout << "King";
                break;
        }
    }

    switch (suitIndex) {
        case 0:
            cout << "Clubs";
            break;
        case 1:
            cout << "Diamonds";
            break;
        case 2:
            cout << "Hearts";
            break;
        case 3:
            cout << "Spades";
            break;
    }
    cout << "." << endl;

    return 0;
}
