// Write the program that will ask for the following input from the user:
// Student:
// Program/Course
// Year Lever: (should be integer type)
// Number of units Enrolled: (should be double or float data type)

// Determine the corresponding year name of the student and rate unit as follows:
    // Year Level   Year Name   Rate Per Unit
    // 1            Freshmen    1,500
    // 2            Sophomore   1,800
    // 3            Junior      2,000
    // 4 or 5       Senior      2,300

// Compute the tuition fee as follows:
    // Tuition fee = no. of units enrolled x rate per unit
    // Down payment = 30% of the tuition fee
    // Balance = Tuition fee - down payment

// Assume that the user will not enter a invalid value.

// Sample Input:
    //Student Name:
    // Program/Course:
    // Year Level:
    // No. of Units:

// Sampul Output:
    // ENROLMENT SLIP
    // Student Name:
    // Program/Course:
    // No. of Units:
    // Tuiton Fee: 36800
    // Down Payment: 11040
    // Balance: 25760

#include <iostream>
using namespace std;

int main(){
    // Student Name:
    string studentName;
    // Program/course:
    string course;
    // Year Level: (should be integer type)
    short yearLevel;
    // Number of Units Enrolled: (should be double or float data type)
    double numberOfUnits;
    
    string yearName;
    float ratePerUnit;

// Tuition fee = no. of units enrolled x rate per unit
// Down payment = 30% of the tuition fee
// Balance = Tuition fee - down payment
    float tuitionFee;
    float downPayment;
    float balance;

// Student Name: Maria Blanco
// Program/Course: : Bachelor of Science in Information Technology
// Year Level: 4
// No. of Units: 16
    cout<< "Student Name:" << endl;
    cin>> studentName;
    cout<< "Program/Course:" << endl;
    cin>> course;
    cout<< "Year Level:" << endl;
    cin>> yearLevel;
    cout<< "No. of Units:" << endl;
    cin>> numberOfUnits;

// Determine the corresponding year name of the student and rate unit as follows:
    // Year Level   Year Name   Rate Per Unit
    // 1            Freshmen    1,500
    // 2            Sophomore   1,800
    // 3            Junior      2,000
    // 4 or 5       Senior      2,300
switch(yearLevel){
    case 1:
    yearName = "Freshmen";
    ratePerUnit = 1500;
    break;
    case 2:
    yearName = "Sophomore";
    ratePerUnit = 1800;
    break;
    case 3:
    yearName = "Junior";
    ratePerUnit = 2000;
    break;
    case 4:
    yearName = "Senior";
    ratePerUnit = 2300;
    break;
}

// Compute the tuition fee as follows:
// Tuition fee = no. of units enrolled x rate per unit
// Down payment = 30% of the tuition fee
// Balance = Tuition fee - down payment
    tuitionFee = numberOfUnits * ratePerUnit;
    downPayment = tuitionFee * 0.3;
    balance = tuitionFee - downPayment;

// Sample Input:
// Student Name: Maria Blanco
// Program/Course: : Bachelor of Science in Information Technology
// Year Level: 4
// No. of Units: 16
    cout<< "ENROLLMENT SLIP" << endl;
    cout<< "Student Name:" << studentName << endl;
    cout<< "Program/Course:" << course << endl;
    cout<< "Year Level:" << yearName << endl;
    cout<< "No. of Units:" << numberOfUnits << endl;
    cout<< "Tuition Fee:" << tuitionFee << endl;
    cout<< "Down Payment:" << downPayment << endl;
    cout<< "Balance:" << balance << endl;

    return 0;
    
}
