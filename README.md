# Reverse
//Code by TALHA GULZAR
#include <iostream>
using namespace std;

int main() {
    int num, reverse = 0;

    // Ask user for input
    cout << "Enter a three-digit number: ";
    cin >> num;

    // Check if number is three-digit
    if (num >= 100 && num <= 999) {
        // Reverse the number
        while (num != 0) {
            int digit = num % 10;
            reverse = reverse * 10 + digit;
            num /= 10;
        }

        // Display result
        cout << "Reverse of the number: " << reverse << endl;
    } else {
        cout << "Please enter a three-digit number." << endl;
    }

    return 0;
}

