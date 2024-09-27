# EXPERIMENT 15
# Aim
To study and implement Recursion.
# Software Used
Visual Studio Code
# Theory
Recursion is a technique in which a function is repeatedly called until the given condition is satisfied. 

A function which calls itself is called a recursive function. When it is called it executes a set of instructions and then calls itself. This continues till the condtion is satisfied and recursion is stopped and returns a value.

Base conditiopn is the condition which terminates recursion. The function is called till the base condition is satisfied.

The recursive case refers to how the recursive call appears in the function. The recursive case can include multiple recursive calls or different parameters, so that the base condition is satisfied and the recursion is terminated.

Syntax:

```
return_type recursive_func {
   
       // Base Condition
       // Recursive Case
      
}
```
CODES:

1. Factorial
```
#include <iostream>
using namespace std;
int fact(int n){
    if (n<=1){
        return 1;
    }else{
        return (n * fact(n - 1));
    }
}
int main(){
    int X,n;
    cout<<"Enter a number:";
    cin>>n;
    X=fact(n);
    cout<<"Factorial:"<<X<<endl;
    return 0;
}
```

o/p: 

![image](https://github.com/user-attachments/assets/42f228d4-17ca-4ba0-bbb0-a2b66c39aab9)




2. Sum of numbers 1 to n
```
#include <iostream>
using namespace std;

int add(int n){
if (n<=1){
return 1;
}
else{
return(n+add(n-1));
}
}
int main(){
int X,n;
cout<<"Enter a number:";
cin>>n;
X=add(n);
cout<<"Sum of numbers is:"<<X<<endl;
return 0;
}
```
o/p: 

![image](https://github.com/user-attachments/assets/bc8a8f60-4a4b-49bf-ae25-4c139f860501)




3. Reversing a string
```
#include<iostream>
using namespace std;
void reverse(char *str){
    if (*str){
        reverse(str+1);
        cout<<*str;

    }
}
int main(){
    char s[50];
    cout<<"Enter a string:";
    cin>>s;
    cout<<"Reversed string is:";
    reverse(a);
    cout<<endl;
    return0;
}
```

o/p:

![image](https://github.com/user-attachments/assets/b2bdf6d4-b561-4c3c-96fc-b4f16b7a62f9)




4. Reversing a number
```
#include<iostream> 
using namespace std;

void print_rev(int i) {
    if (i > 0) {  
        cout << (i % 10);  
        print_rev(i / 10);  
    }
}

int main() {
    int i;
    cout << "Enter the number: ";
    cin >> i; 
    print_rev(i);  
    cout << endl;  
    return 0; 
}
```

o/p:

![image](https://github.com/user-attachments/assets/8e65e207-8aa9-46f1-9e32-d46e9f116515)





# Conclusion
The above codes show how recursion can effectively reverse strings and digits, compute factorials and sums, and improve code readability. They demonstrate how elegant and useful recursion is as a programming tool.
