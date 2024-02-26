//pointers.cpp

#include <iostream>
using namespace std;

class STUDENT {
public:
    string name;
    int age;

    STUDENT(string n, int a) {
        name = n;
        age = a;
    }

    void display() {
        cout << "Name: " << name << ", Age: " << age << endl;
    }
};

int main() {
    // create a new STUDENT object
    STUDENT student1("John Doe", 18);

    // create a pointer to a STUDENT object
    STUDENT* pStudent = &student1;

    // access members of the STUDENT object using the pointer
    pStudent->display();
    cout << "Name: " << pStudent->name << ", Age: " << pStudent->age << endl;

    return 0;
}
