# Experiment 15

**Aim:** <br>
To study and implement Recursion. <br>
<br>
**Theory:** <br>
In C++, recursion is executed through when a function calls itself. The concept itself is essentially the same as in other programming languages; the function ultimately calls itself with changed arguments consistently until a base case is reached at which point it will stop calling itself and begin returning results along the route of recursive calls.  <br>
<br>
Properties of Recursion: <br>
&#8594; _Base Case:_ Recursion stops when there is a condition. <br>
&#8594; _Recursive Case_: It is a solution to sub problems through recursive call. <br>
&#8594; _Call Stack:_ The modules that contain each separate function in memory. <br>
&#8594; _Overhead:_ Non-direct calculations that bite into the call and storage space. <br>
&#8594; _Memory Consumption:_ Excessive levels of recursion may lead to rampant overflow of state. <br>
&#8594; Tail Recursion: This is a type of recursion where the last action is that of invoking another instance of the same function, and thus optimizations can be made. <br>
&#8594; Direct/Indirect Recursion: This is an instance of recursion in which the function invokes itself directly or indirectly. <br>
&#8594; Multiple Recursive Calls: Functions can perform more than one recursive call. <br>
&#8594; Backtracking: This method is used in algorithms that use multiple paths to find solutions. <br>
<br>

**Code:** <br>
<br>
a.<br>

```
#include <iostream>
using namespace std;
int fact(int n)
{
    if (n<=1)
    {
        return 1;
    }
    else
    {
        return (n*fact(n-1));
    }
}
int main()
{
    int x,n;
    cout<<"Enter a number: ";
    cin>>n;
    x= fact(n);
    cout<<n<<"!: "<<x;
}


```
<br>
b.<br>

```
#include <iostream>
using namespace std;
int add(int n)
{
    if (n<=1)
    {
        return 1;
    }
    else
    {
        return (n+add(n-1));
    }
}
int main()
{
    int x,n;
    cout<<"Enter a number: ";
    cin>>n;
    x= add(n);
    cout<<x;
}

```
<br>
c.<br>

```
#include <iostream>
#include <string>
using namespace std;
void rev(char *str)
{
    if (*str)
    {
        rev(str+1);
        cout<<("%c",*str);

    }

}
int main()
{
    char s[50];
    cout<<"Enter a string: ";
    cin>>s;
    rev(s);
}

```
<br>
d.<br>

```
#include <iostream>
#include <string>
using namespace std;
void revn(int i)
{
    if (i>0)
    {
        cout<<i%10;
        revn(i/10);
        

    }

}
int main()
{
    int i;
    cout<<"Enter a number: ";
    cin>>i;
    revn(i);
}

```
<br>

**Outputs:**  <br>
<br>
a.<br>
![image](https://github.com/user-attachments/assets/e2d71944-46a8-43bd-874f-7aa37cc61dae)

 <br>
b.<br>
![image](https://github.com/user-attachments/assets/59bbf3d6-afbe-4949-8480-50cac05e2c4e)

 <br>
c.<br>
![image](https://github.com/user-attachments/assets/5c59e3f8-3427-41f2-8958-2c81fe4cf630)

 <br>
d.<br>
![image](https://github.com/user-attachments/assets/bc477e65-09a5-48fb-b93d-97ff381740c9)

 <br>



<br>

**Conclusion:** <br>
&#8594; We learnt about recursion in C++. <br>
&#8594; We learnt the use case of recursion in C++. <br>
*******
<br>
