# First-Project
Jeremy Tajiri's first C++ project for CISC 191.
- Assisted by Krish Adiraj 


One thing Krish and I learned: When dividing integers in C++, it automatically cuts off the decimal part. So, in order to keep the decimals, we had to turn it into a double with (double) or static_cast (). 

One bug we fixed: In the discount program, 15 / 100 gave us 0 because of integer math. We fixed it by changing it to double discountPercent / 100

