# *task1*
## **fibonacci sequence**
to know all about fibonacci click [here](https://en.wikipedia.org/wiki/Fibonacci_number) 

![alt text](https://cdn.insteading.com/wp-content/uploads/2020/12/shell.jpg)
### here are some answers for fibonacci sequence
1. first answer (*recursion*)

`#include <iostream>`  
`using namespace std;  `
  
`int fib(int n)`  
`{  `
  `  if (n <= 1)`  
       ` return n;  `
 `return fib(n - 1) + fib(n - 2);`  
`}  `
  
`int main()`  
`{  `
  `  int n; ` 
  `cin>>n;  `
  `cout << fib(n);`  
` return 0;  `
`}`

  2.second answer (vector)

`#include <iostream>`  
`#include <vector>  `
  
`using namespace std;`  
`int main(){  `
  `  int n; ` 
  `cin>>n;  `
`vector<int> v {0,1};`  
  
  
 `for (int i = 2; i <= n; i++){ ` 
  `      v[i] = v[i - 1] + v[i - 2];`  
  `}  `
  
  
  `  cout<<v[n]; ` 
 `return 0;`  
`}`

3.third answer

`#include<bits/stdc++.h>`

`using` `namespace` `std;`

`int` `fib(``int` `n)`

`{`

`int` `a = 0, b = 1, c, i;`

`if``( n == 0)`

`return` `a;`

`for``(i = 2; i <= n; i++)`

`{`

`c = a + b;`

`a = b;`

`b = c;`

`}`

`return` `b;`

`}`

`int` `main()`

`{`
`int n`

`cin>>n;`

`cout << fib(n);`

`return` `0;`

`}`


## space and time complexity table

| method | space complexity | time complexity |   
| ----------- | ----------- |   ----------- |   
| first answer | O(n) if we consider the function call stack size, otherwise O(1). |  ** Exponential ** as every function calls two other functions. |   
| second answer |  | O(n)  |   
| third answer | O(1) | O(n) |   




