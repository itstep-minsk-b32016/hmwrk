#include <iostream>
#include <iomanip>
using namespace std;

int main(int argc, char *argv[])
{
	setlocale(LC_ALL, "rus");
	const unsigned first = 3, second_col = 3;
	int mass1[first][second_col];
	cout << "Введите число : \n";
	int a; cin >> a;

	for (int i = 0; i < first; i++)
	{
		for (int j = 0; j < second_col; j++)
		{
			if (i == 0 && j == 0)
			{
				mass1[i][j] = a;
			}
			else if (i == 0) 
			{
				mass1[i][j] = mass1[i][j - 1] * 2; // Если +1 то задание N2
			}
			else if (i > 0 && j == 0)
			{
				mass1[i][j] = mass1[i - 1][j + (second_col - 1)] * 2; // Если +1 то задание N2
			}
			else if (i > 0 && j > 0)
			{
				mass1[i][j] = mass1[i][j - 1] * 2; // Если +1 то задание N2
			}
			cout << setw(5) << mass1[i][j] << " ";
		}
		cout << endl;
	}
}
