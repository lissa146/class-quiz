# class-quiz
#include<iostream>
using namespace std;

class Student {
private:
	string name;
	int scigrade;
	int mathgrade;
	int englishgrade;
	int num;
	//int takeDam;
public:
	Student(int s, int m, int e, string n);
	void printinfo();
	void getAverage();
};

int main() {
	Student Alice(100, 50, 50, "Alice");
	Alice.printinfo();
	Alice.getAverage();
}

Student::Student(int s, int m, int e, string n) {
	scigrade = s;
	mathgrade = m;
	englishgrade = e;
	name = n;
}


//}
void Student::printinfo() {
	cout << name << endl;
	cout << "science grade"<< scigrade << endl;
	cout << "math grade"<<mathgrade << endl;
	cout << "english grade"<< englishgrade << endl;
}

void Student::getAverage() {
	float  answer = scigrade + mathgrade + englishgrade / 3;
	cout << answer << endl;

}
