# CDS.EXP-11
## Aim:
**To study and implement Classes and Objects..**

## Software:
`Microsoft VSCode`

## Theory:
Class -> A class is a usser-defined data type, which holds its own data members and member functions, which can be accessed and used by creating an instance of that class.

Object-> When a class is defined, only the specification for the object is defined, no memory or storage is allocated. To use the data and access functions defined in the clss, we need to create objects.

In C++, there are three access specifiers that are:
(1) Public: Members declared as public can be accessed from outside the class.
(2) Private: Members declared as private can only be accessed within the class itself.

(3) Protected: Members declared as protected cn be accessed within the class and by derived classes.
Any changes made to the parameters within the function are directly reflected in the original values outside the function.
## Code: 11A
```
//AKALP SARKAR
//ENTC B2
//EXP 11A
//23070123116
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h = 2.0;
    double b = 3.0;
    double l = 4.0;
};
int main()
{
  cuboid c1;
  double vol = c1.h * c1.b * c1.l;
  cout<<"Volume "<<vol<<endl;
}
```
## Output:
![Output11A](https://github.com/user-attachments/assets/d899a6c6-d872-46d5-a216-0262db1cc6eb)!

## Code: 11B
```
//AKALP SARKAR
//ENTC B2
//EXP 11B
//23070123116
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h = 2.0,b = 3.0,l = 4.0;
    double volume()
    {
        double vol = h * b * l;
        cout<<"Volume "<<vol<<endl;
    }

};
int main()
{
    cuboid c1;
    c1.volume();
  
}
```

## Output:
![Output11B](https://github.com/user-attachments/assets/5fbef6c0-1f0e-47da-8f5d-ae8ea56e58fd)


## Code:11C
```
//AKALP SARKAR
//ENTC B2
//EXP 11C
//23070123116
# include<iostream>
using namespace std;
class cuboid
{
    private:
    double h = 3.0,b = 2.0,l = 4.0;
    public:
    double volume()
    {
        double vol;
        vol = h * b * l;
        cout<<"Volume "<<vol<<endl;
    }

};
int main()
{
    cuboid c1;
    c1.volume();
  
}
```

## Output:
![Output11C](https://github.com/user-attachments/assets/ce71710f-f49b-481e-8507-82e1ee241ff4)

## Code: 11D
```
//AKALP SARKAR
//ENTC B2
//EXP 11D
//23070123116
# include<iostream>
using namespace std;
class cuboid
{
    private:
    double h = 2.0,b = 3.0,l = 4.0;
    public:
    double volume()
    {
        double vol;
        vol = h * b * l;
        return vol;
    }

    void disp(double vol)
    {
        cout<<"Volume "<<vol<<endl;

    }

};
int main()
{
    cuboid c1;
    double v = c1.volume();
    c1.disp(v);
  
}
```

## Output:
![Output11D](https://github.com/user-attachments/assets/cdc40975-3dd1-4bf8-b1eb-e2fe1117faed)

## Code: 11E
```
//AKALP SARKAR
//ENTC B2
//EXP 11E
//23070123116
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h,b,l;
    void input()
    {
        cout<<"Enter the length: ";
        cin>>l;
        cout<<"Enter the breadth: ";
        cin>>b;
        cout<<"Enter the height: ";
        cin>>h;
    }
    double volume()
    {
        double vol;
        vol = h * b * l;
        return vol;
    }

    void disp(double vol)
    {
        cout<<"Volume "<<vol<<endl;

    }

};
int main()
{
    cuboid c1;
    c1.input();
    double v = c1.volume();
    c1.disp(v);
  
}
```
## Output:
![Output11E](https://github.com/user-attachments/assets/0e5e23db-b37b-4fd1-a99b-d3c9ffd135d3)

### Conclusion:
In this experiment, i learnt about classes and objects in C++ and performed programs using them and also learnt about local variables and global variables.
