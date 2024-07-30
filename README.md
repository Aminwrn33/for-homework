#include <iostream>

using namespace std;

int main()
{
    int i, j, n;
    const int size = 10;
    const int olcu = 21;
    const int tap4size = 10;

    cout << "Tapsiriq 1\n\n";
    cout << "\nDaxil et(10-dan basqa daxil etme 10 yaz bura):";
    cin >> n;
    for (i = 1; i <= n; i++)
    {
        cout << "\n";
        for (j = 1; j <= n; j++)
        {
            if (i == 1 || i == n || j == 1 || j == n)
                cout << " *";
            else
                cout << "  ";
        }
        cout << endl;
    }
    cout << "\n\n";

    cout << "Tapsiriq 2\n\n";

    for (int i = 0; i < size; ++i) {
        for (int j = 0; j < size; ++j) {
            cout << " *";
        }
        cout << endl;
    }
    
    cout << "\n\n";

    cout << "Tapsiriq 3\n\n";

    for (int i = 0; i < olcu; ++i) {
        for (int j = 0; j < olcu; ++j) {

            if (i == 0 || i == olcu - 1 || j == 0 || j == olcu - 1 || i == olcu / 2 || j == olcu / 2) {
                cout << " *";
            }
            else {
                cout << "  ";
            }
        }
        cout << endl;
    }

    cout << "\n\n";

    cout << "Tapsiriq 4\n\n";

    for (int i = 0; i < tap4size; ++i) {
        for (int j = 0; j < tap4size; ++j) {

            if (i == 0 || i == tap4size - 1 || j == 0 || j == tap4size - 1 || i == j || i + j == tap4size - 1) {
                cout << "* ";
            }
            else {
                cout << "  ";
            }
        }
        cout << endl;
    }




}





