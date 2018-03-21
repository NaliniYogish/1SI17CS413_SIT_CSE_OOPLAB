#include <iostream>
using namespace std;

//enum color{red,yellow,green};
enum color{red=1,yellow=2,green=3};

int main()
{
    color val;
    int iChoice;
    
    cout << "\nEnter color state\n";
    cin >> iChoice;

//    val = iChoice;    /*invalid conversion*/
    val = (color)iChoice;
    switch(val)
    {
        case red:   cout<< "Halt" << endl;
                    break;
        case yellow:   cout<< "Ready" << endl;
                    break;
        case green:   cout<< "Go" << endl;
                    break;
    }
    return 0;
}
