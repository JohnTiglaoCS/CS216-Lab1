/* John Tiglao
Description: You are doing a summer job that is 5 weeks long and you make $15.50 an hour so you can buy supplies for your school.
Date: 9/3/2024
*/

#include <iostream>
using namespace std;

int main() {
	double IncomeBeforeTaxes, TaxRate, IncomeAfterTaxes;
	double SpendingOnClothesAndAccessories, SpendingOnSchoolSupplies, SpendingBonds;
	double ParentsBonds, TotalSpent, TotalSaving;

	cout << "Summer job is $15.50 ";
	cin >> IncomeBeforeTaxes;
	cout << "14% "; 
	cin >> TaxRate;

// Your income after taxes 
	IncomeAfterTaxes = IncomeBeforeTaxes * (1 - TaxRate / 100.0);

// Money is spent in each categories
	cout << "10% ";
	cin >> SpendingOnClothesAndAccessories;
	cout << "1% ";
	cin >> SpendingOnSchoolSupplies;
	cout << "25% ";
	cin >> SpendingBonds;
	cout << "0.25 ";
	cin >> ParentsBonds;

// The total money spent 
	TotalSpent = SpendingOnClothesAndAccessories + SpendingOnSchoolSupplies + SpendingBonds;

// After Tax 
	TotalSpent = (IncomeAfterTaxes - TotalSpent) + ParentsBonds;



}
