# AIM

To learn about inheritance and its type in c++.

# Software Used

VS Code and Cpp Online Compiler

# Problem Codes

1.) Write a c++ code to do single inheritence.

2.) Write a c++ code to do multiple inheritanc.

# Theory

The capability of a class to derive properties and characteristics from another class is called Inheritance. Inheritance is one of the most important features of Object Oriented Programming in C++. In this article, we will learn about inheritance in C++, its modes and types along with the information about how it affects different properties of the class.

# Problem Codes

```javascript

//SINGLE INHERITANCE
#include <iostream>
using namespace std;

class Bands {

public :
string bd;
string sr;
void genre(){

    cout<<"Enter the name of band: "<<endl;
    cin>>bd>>sr;
    

}
};

class Lz : public
Bands {
    public:
     int est;
    void estd(){
       
    cout<<"Estalished: "<<endl;
    cin>>est;
    
}
void display(){
    cout<< "The band is: "<<bd<<" "<<sr<<endl;
    cout<<"Established: "<<est<<endl;

}
};
int main()
{
    Lz d;
    d.genre();
    d.estd();
    d.display();
    
    return 0;
}

//MULTIPLE INHERITANCE
#include <iostream>
using namespace std;

class Engine {
    public :


    void start(){
        cout<< "Engine starts"<<endl;
        

    }
};
class Transmission{
    public:
   void shiftGear(){
    cout<<"Transmission shifts gear"<<endl;
   }
   };

    class Car : public Engine, public Transmission {
        public:
        void drive(){
            cout<<"Card is driving"<<endl;
        }
    };

int main()

{
    Car d;
    d.shiftGear();
    d.drive();
    return 0;
}
```
//MULTILEVEL INHERITANCE
# include<iostream>
using namespace std;

class planets {
    public:
    string st, ju;

    void gas(){
        cout<< "The planet which are gas giants: "<<endl;
        cin>>st>>ju;
        
    }
};
class li :
public
planets{
    public:
    string et;
    void life(){
    
    cout<< " Planet with life: "<<endl;
    cin>>et;
    
}
};

class SolarSystem : public
li{
    public:
    string cm,cl;
    void comets(){
        cout<< "The home of comets: "<<endl;
        cin>>cm>>cl;
        
    }


void display(){
     cout<< st<<" & "<<ju << " are gas giants."<<endl;
  
     cout<< et <<" is the planet with life."<<endl;
  cout<< cm <<" "<< cl<<" is the home of comets"<<endl;
}
};
int main (){
    SolarSystem d;
    d.life();
    d.comets();
    d.gas();
    d.display();
}


//HIERARCHICAL INHERITANCE
# include<iostream>
using namespace std;

class Galaxy {
    public:
    string gy,wy,gr,cr;
    void gl(){
        cout<<" Which Galaxy: "<<endl;
        cin>>gy>>wy;
        

    }
    void display(){
        cout<< "Galaxy: "<< gy<<" "<<wy<<endl;
        cout << "Group: "<<gr<<" "<<cr<<endl;

    }
};

class Earth: public Galaxy{
    public:
   
    void gp(){
        cout<< "Which Group: "<<endl;
        cin>>gr>>cr;
        cout << "Group: "<<gr<<" "<<cr<<endl;
    }
};
class NGC: public Galaxy{
       public:
    
    void go(){
        cout<< "Which Group: "<<endl;
        cin>>gr>>cr;
        
    }

};

int main(){
    Earth d;
    NGC c;
    d.gl();
    d.gp();
    d.display();

    c.gl();
    c.go();
    c.display();
    return 0;

}
```


# Output
## 1) Single Inheritance
![Exp 14 Single Inheritance](https://github.com/user-attachments/assets/6be82ca1-b9a5-4072-a1fa-8be82919059a)

## 2) Multiple Inheritance
![Exp 14 Multiple Inheritance](https://github.com/user-attachments/assets/e6651422-4161-4307-93b4-6186bcbcf156)
## 3) Multilevel Inheritance
![Exp 14 Multilevel Inheritance](https://github.com/user-attachments/assets/c67bc5d5-f0a5-40a8-9b2b-475c1d35b079)

## 4) HIERARCHICAL INHERITANCE
![Exp 14 Hierarchical Inheritance](https://github.com/user-attachments/assets/0b5560bd-4705-4f6a-9e5d-13d7109cdde1)


# Conclusion
We learnt to do multiple and single inheritance.
