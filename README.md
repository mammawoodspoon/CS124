/***********************************************************************
* Program:
*    Project 02, Monthly Budget
*    Brother Ellsworth, CS124
* Author:
*    Erin Humphreys
* Summary: 
*    This is a personal finance management program. This program will manage 
*    finances for one month.
*    
*    
*    
*    
*
*    Estimated:  6.0 hrs   
*    Actual:     7.0 hrs
*      The most difficult part has been getting the code correct.
************************************************************************/

#include <iostream>
#include <iomanip>
using namespace std;

/**********************************************************************
 * Main will call the get and display functions and hold the input values 
 ***********************************************************************/
int main()
{
   cout << "This program keeps track of your monthly budget" << endl;
   cout << "Please enter the following:\n";
   // set the configuration for output to display money
   cout.setf(ios::fixed);
   cout.setf(ios::showpoint);
   cout.precision(2);

   // get monthly income
   float income;
   cout << "\tYour monthly income: ";
   cin  >> income;
  
   // get budgeted living expenses
   float budgetLiving;
   cout << "\tYour budgeted living expenses: ";
   cin  >> budgetLiving;
  
   // get actual living expenses
   float actualLiving;
   cout << "\tYour actual living expenses: ";
   cin  >> actualLiving;
     
   // get actual taxes withheld
   float taxes;
   cout << "\tYour actual taxes withheld: ";
   cin  >> taxes;
     
   // get actual tithe offerings
   float tithing;
   cout << "\tYour actual tithe offerings: ";
   cin  >> tithing;
     
   // get actual other expenses
   float other;
   cout << "\tYour actual other expenses: ";
   cin  >> other;
   cout << "\n";    

   cout << "The following is a report on your monthly expenses\n";
   cout << "\tItem"  
        << setw(24)  << "Budget" 
        << setw(16)  << "Actual" 
        << endl;
   cout << "\t=============== " 
        << setw(12)  << "==============="  
        << setw(16)  << "==============="
        << endl;
   cout << "\tIncome" 
        << setw(11)  << "$"  
        << setw(11)  << income     
        << setw(5)   << "$"      
        << setw(11)  << income         
        << endl;
   cout << "\tTaxes" 
        << setw(12)  << "$"  
        << setw(11)  << "0.00"     
        << setw(5)   << "$"      
        << setw(11)  << taxes         
        << endl;
   cout << "\tTithing" 
        << setw(10)  << "$"  
        << setw(11)  << "0.00"     
        << setw(5)   << "$"      
        << setw(11)  << tithing         
        << endl;
   cout << "\tLiving" 
        << setw(11)  << "$"  
        << setw(11)  << budgetLiving     
        << setw(5)   << "$"      
        << setw(11)  << actualLiving         
        << endl;
   cout << "\tOther" 
        << setw(12)  << "$"  
        << setw(11)  << "0.00"     
        << setw(5)   << "$"      
        << setw(11)  << other         
        << endl;   
   cout << "\t=============== " 
        << setw(12)  << "==============="  
        << setw(16)  << "==============="
        << endl;
   cout << "\tDifference" 
        << setw(7)   << "$"  
        << setw(11)  << "0.00"     
        << setw(5)   << "$"      
        << setw(11)  << "0.00"         
        << endl;
   
   return 0; 
}

