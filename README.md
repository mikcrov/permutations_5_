#include <iostream>
#include <vector>
using namespace std;



int main() {
	int n;
	cout << "enter n: ";
	cin >> n;
	cout << "\n";

	vector<int> numbers;


	if (n == 1 || n == 2 || n == 3) {
		cout << "NO SOLUTION";
	}
	else {
		for (int i = 2; i <= n; i += 2) {
			numbers.push_back(i);
		}
		for (int i = 1; i <= n; i += 2) {
			numbers.push_back(i);
		}

		for (int number : numbers) {
			cout << number << " ";
		}
	}

	return 0;
}
