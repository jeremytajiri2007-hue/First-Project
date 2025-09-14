## Task A1
Cpp
#include <iostream>
using namespace std;

int main() {
    int a, b, c;
    cin >> a >> b >> c;

    cout << "a + b  c = " << a + b  c << endl;
    cout << "(a + b)  c = " << (a + b)  c << endl;
    cout << "a / b  c = " << a / b  c << endl;
    cout << "a / (b  c) = " << a / (b  c) << endl;

    return 0;
}

## Task A2
Cpp

#include <iostream>
#include <iomanip>
using namespace std;

int main() {
    double balance;
    int deposits;
    int withdrawals;

    cin >> balance >> deposits >> withdrawals;

    balance = balance + deposits  25.50;
    balance = balance - withdrawals  12.75;

    cout << fixed << setprecision(2);
    cout << "Final balance = " << balance << endl;

    return 0;
}

## Task B1

Cpp

#include <iostream>
using namespace std;

int main() {
    int s1, s2, s3;
    cin >> s1 >> s2 >> s3;

    int sum = s1 + s2 + s3;
    cout << "Raw average (implicit): " << sum / 3 << endl;
    cout << "Correct average (explicit cast): " << (double) sum / 3 << endl;

    return 0;
}

## Task B2

Cpp

include <iostream>
include <iomanip>
using namespace std;

int main() {
    int wins, games;
    cin >> wins >> games;

    if (games == 0) {
        cout << "No games played." << endl;
    } else {
        double pct = (double) wins / (double) games  100.0;
        cout << fixed << setprecision(1);
        cout << "Win% = " << pct << "%" << endl;
    }

    return 0;
}

## Part C

Cpp

include <iostream>
include <iomanip>
using namespace std;

int main() {
    double hours, rate;
    cin >> hours >> rate;

    double regHours;
    if (hours > 40) {
        regHours = 40;
    } else {
        regHours = hours;
    }

    double otHours;
    if (hours > 40) {
        otHours = hours - 40;
    } else {
        otHours = 0;
    }

    double gross = regHours  rate + otHours  rate  1.5;
    double tax = gross  0.18;
    double benefits = 35.0;
    double net = gross - tax - benefits;

    cout << fixed << setprecision(2);
    cout << "Regular: " << regHours << ", Overtime: " << otHours << endl;
    cout << "Gross: $" << gross << endl;
    cout << "Tax (18%): $" << tax << endl;
    cout << "Benefits: $" << benefits << endl;
    cout << "Net: $" << net << endl;

    return 0;
}

## Part D

Cpp

include <iostream>
include <iomanip>
using namespace std;

int main() {
    int items;
    double price;
    cout << "Enter items and price: ";
    cin >> items >> price;

    double total = items  price;

    int discountPercent = 15;
    double discount = total  ((double) discountPercent / 100);

    double shipping = 5 + 2  items;
    double afterDiscount = total - discount;

    if (afterDiscount >= 100) {
        shipping = 0;
    }

    cout << fixed << setprecision(2);
    cout << "Total: $" << total << endl;
    cout << "Discount: $" << discount << endl;
    cout << "Shipping: $" << shipping << endl;
    cout << "Grand Total: $" << (afterDiscount + shipping) << endl;

    return 0;
}
