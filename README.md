# EXP-7

## Aim:
**To study and implement C++ Arrays and Strings..**

## Software:
`Microsoft VSCode`

## Theory:
Array: • An arry is a fixed-size sequential collection of the elemnts of same data type. It consists of continuous memory locations. • The array's indexes begin at 0. Meaning that the first item saved at index 0 is [0]. • The final element of an array with size n is kept at index (n-1).


## Code: 7A
```
//KANWALJEET SINGH
//ENTC B2
//EXP 7A
//23070123124
#include<iostream>
using namespace std; 

// Program to print an array. 
int main() {
    int i;
    int a1[5]={19, 20, 5, 6, 7};
    int a2[5]={5,6,9,0,6};
    cout<<"Array is: ";

    for(i=0; i<5; ++i) {
        cout<<"Array is: "<<a1[i]<<" "<<"\n";
    }
    for(i=0; i<5; ++i) {
        cout<<"Array is: "<<a2[i]<<" "<<"\n";
    }
    return 0;
}
}
```
## Output:
![image](https://github.com/user-attachments/assets/1baf2841-f9b9-4bdd-9385-01ccf12fb557)



## Code: 7B 
```
//KANWALJEET SINGH
//ENTC B2
//EXP 7B
//23070123124
#include <iostream>
#define S 4
using namespace std;

int main() {
    int array1[S];
    //take input from user
    cout << "Enter " << S << " elements of array: ";
    for (int index = 0; index < S; index++) {
        cin >> array1[index];
    }
  cout << endl;

    // display entered array ekements
    for (int j : array1) {
        cout << j << "  ";
    }

   return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/3ac84316-7e56-45c1-9280-707292d26df0)



## Code: 7C 
```
//KANWALJEET SINGH
//ENTC B2
//EXP 7C
//23070123124
int main() {
    int i,n;
    cout<<"Enter the size of array: ";
    cin>> n;
    int a[n]; 
    //create array
    for(i=0;i<n;i++)
    {
        cout<<"Enter elements "<<i+1<<": ";
        cin>>a[i];
    }
    //display input array
     cout<<"Array entered by the user is: ";
    for(i=0;i<n;i++)
    {
        cout<<a[i]<<"";
    }

    //reverse array
    cout<<"\n Reverse of the entered array is: "; 
    for (i=n-1; i>=0; i--) {
        cout<<a[i]<<"";
    }
    return 0; 
}
```
## Output:
![image](https://github.com/user-attachments/assets/7725fc56-4a69-438d-aa97-cb1bca28dbf1)



## Code: 7D 
```
//KANWALJEET SINGH
//ENTC B2
//EXP 7D
//23070123124

#include<iostream>
using namespace std;

int main() {
    int marks[5], i, j, num, a=0, count=0;
    for(i=0;i<5;i++) {
        cout<<"Enter element-"<<i+1<<": ";
        cin>>marks[i];
    }
    cout<<"Enter element to be searched: ";
    cin>>num;
    for(j=0;j<5;j++) {
        if(marks[j]==num) {
            cout<<"Position of "<<num<<": "<<j+1<<endl;
            count++;
            a=1;
        }
    }
    if(a==0) {
        cout<<"Element not present";
    }
    else if(a==1) {
        cout<<"Element is present: "<<count<<" times";
    }
}
```
## Output:
![image](https://github.com/user-attachments/assets/f985ffcc-4c2a-4265-90b3-aaf5acf45593)

## Code 7E
```
#include <iostream>
using namespace std;

int main() {
    
  // declare and initialize an array 
  double numbers[] = {7.5, 2.5, 3.6, 5.12, 7.35, 24.27};

  double sum = 0.0;
  double count = 0.0;
  double average;

  cout << "The numbers are: ";

  //  print array elements use of range-based for loop
  for (const double n : numbers) {
    cout << n << "  ";
    //  calculate the sum
    sum += n;
    // count the no. of array elements
    ++count;
  }
  // print the sum
  cout << "\nSum = " << sum << endl;

  // find the average
  average = sum / count;
  cout << "\nTheir Average = " << average << endl;
  return 0;
}
```
## Output:
![image](https://github.com/user-attachments/assets/3c443243-638c-447f-830c-63126c31e6d4)


## Code 7F.
```
// Finding minimum and maximum element of an array.          

#include<iostream> 
using namespace std; 

int main() {
    int n, i, max=0;  
    cout<<"Enter the number of elements: ";
    cin>>n;
    int a[n];
    for(i=0; i<n; i++) 
    {
        cout<<"Element "<<i<<" is: ";
        cin>>a[i];
    }
    for (i=0;i<n; i++) 
    {
        if (a[i]>max) 
        {
            max=a[i];
        }
    }
    int  min=a[0]; 
    for (i=0; i<n;i++) 
    {
        if (min>a[i]) 
        {
            min=a[i];
        }
    }
    cout<<"Maximum: "<<max<<"\n"<<"Minimum: "<<min;
}
```
## Output:
![image](https://github.com/user-attachments/assets/5a739d56-3592-4f9a-ba74-fbc9452db5b0)

## Code 7G.
```
#include<iostream> 
#include<string>
using namespace std; 

int main() 
{
    string a;
    cout<<"Enter any word: "; 
    cin>>a;
    cout<<"Entered string is "<<a<<"."<<"\n";
    return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/2c707a25-40f0-4790-807c-a08ec7462f5e)

## Code 7H
```
#include<iostream>
#include<string>
using namespace std;
int main() {
string a, b;
cout<<"Enter strings: ";
cin>>a>>b;
cout<<"CONCATENATION: "<<a+b;

return 0;
} 
```
## Output:
![image](https://github.com/user-attachments/assets/ce4b79dd-dbb1-40f6-9082-fa10f85a5a74)

## Code 7I.
```
#include<iostream>
#include<string>
using namespace std;
int main() {
string a;
cout<<"Enter string: ";
cin>>a;
int i;
for(i=a.length()-1;i>=0;i--) {
cout<<a[i];
}
return 0;
}
```
## Output:
![image](https://github.com/user-attachments/assets/5497a3a7-f400-4d3d-b595-65f4b251c0b1)

## Code 7J.
```
#include<iostream>
#include<string>
using namespace std;
int main() {
string a;
cout<<"Enter a string: ";
cin>>a;
int n=a.length(), i, flag=0;
for(i=0;i<a.length();i++){
if(a[i]==a[n-1]){
flag=1;
}
n--;
}
if(flag==1){
cout<<a<<" is palindrome";
}
else{
cout<<a<<" is not palindrome";
}
}
```

## Output:
![image](https://github.com/user-attachments/assets/b12d6c5f-8a68-4c36-a964-109a45ca17e9)
