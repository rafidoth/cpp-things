# CPP & STL


### Table of Contents
- [Structure](#structure)
- [Pair](#pair)


## Pair
- Initializing Pair
```

```

## Structure

It can be called a custom data type simply. To store more than one data type we use structure. 

- Declaration of Structure
```
#include<bits/stdc++.h> 
using namespace std;


struct Point{
    int x;
    int y;
};



int main(){
    struct Point p1;
    cout << p1.x << " "<< p1.y << "\n"; // will give error (Not initialized yet)
}

```
- Initializing Value & Accessing value
```
#include<bits/stdc++.h> 
using namespace std;


struct Point{
    int x;
    int y;
};



int main(){
    struct Point p1;
    p1.x = 10;
    p1.y = 23;
    struct Point p2;
    p2.x = 2;
    p2.y = 4;
    cout << p1.x << " "<< p1.y << "\n";
    cout << p2.x << " "<< p2.y << "\n";
}

```

- Storing instance of structures in array or other containers like vector , map etc.
```
#include<bits/stdc++.h> 
using namespace std;


struct Point{
    int x;
    int y;
};



int main(){
    Point points[5];
    cout << "Enter 5 points"<<"\n";
    for(int i =0;i<5;i++){
        cin >> points[i].x >> points[i].y;
    }

    for(int i =0;i<5;i++){
        cout << "Point "<< i+1<<"->";
        cout << points[i].x << " "<< points[i].y<<"\n";
    }
}

```

- Pointer & Sructure 
```
#include<bits/stdc++.h> 
using namespace std;


struct Point{
    int x;
    int y;
};



int main(){
    struct Point p1;
    p1.x = 10;
    p1.y = 20;
    
    Point *ptr = &p1;
    cout << ptr->x << " "<< ptr->y << "\n";

}

```