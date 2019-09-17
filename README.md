# lab6-
#include <iostream>
#include <string>
#include <conio.h>

using namespace std;

int string_find(string str, char s)
{
	int counter = 0;

	for (int i(0); i<str.length() - 1; i++)
	{
		if (str[i] == s)
			counter++;
	}
	return counter;
}

int main()
{
	char s;
	string str1;
	string str2;
	cout << "enter two  string: " << endl;
	cin >> str1;
	cin >> str2;

	cout << "enter the symbol for search: " << endl;
	cin >> s;

	cout<<"1. caunter= "<<string_find(str1, s)<<endl;

	cout << "2.concatenation:  " << str1  + str2<<endl;

	cout << "3.length first_string=\t" << str1.length() << endl;
	cout << "  length second_sting=\t" << str2.length() << endl;

	if (str1 == str2)
		cout << "4.comparison\t string are equal" << endl;
	else
		cout << "4.comparison\t string are unequal" << endl;

	for (int i(0); i < str1.length(); i++)
	{
		if (str1[i] == 'a')
			str1[i] = 'b';
	}
	cout << "5." << str1 << endl;

	str1[1] = 'a';
	str1[4] = 'a';

	cout << "6." << str1 << endl;

	


	_getch();
	return 0;
}
