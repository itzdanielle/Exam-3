# Exam-3
#include <iostream>
using namespace std;

int main() {
  const int MIN_VALUE = 30;
  const int MAX_VALUE = 80;
  float num;
  cout << "Input numbers to square. Input -1 to stop." << endl;
  cout << "Enter a number that you would like to square" << endl;
  cin >> num;
  int square;
  
   while ( num != -1)  {
     square = num * num;
    cout << "Square is : " << square << endl;
    cout << "Enter a number that you would like to square" << endl;
    cin >> num;
    
     }
  


  int tries = 0;
   tries = num + num + num;
  int sum;
    if (num == -1) {
   sum = square + square +square + square/4;
  cout << "You entered " << tries << endl;
  cout << "The sum of all the squares is " << sum << endl;
  }
  if (sum <= MIN_VALUE) {
  cout << "Warning: The sum of the squares is less than the minimum value." << endl;
  }
  if (sum >= MAX_VALUE) {
    cout << "Warning: The sum of the squares is greater than the maximum value." << endl;
  }
}
