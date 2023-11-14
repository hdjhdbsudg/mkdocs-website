---
tags:
  - Code/Cpp
---


### Tổng quan
Cho phép chuyển đổi các kiểu dữ liệu khác nhau và chuỗi.
1. Tách chuỗi
2. Ghép chuỗi
![[Excalidraw/stringstream]]
Ví dụ:
```cpp 
string s = "123 456 789";
    stringstream ss(s);
    int a, b, c;
    ss >> a >> b >> c;
    cout << a << ' ' << b << ' ' << c << endl;
    return 0;
// output
// 123 456 789

stringstream để tách chuỗi thành 3 số và lưu vào a, b, c.
```cpp
#include <iostream>
#include <sstream>
#include <string>
using namespace std;
int main() {
  string sentence = "COUNT words in sentence using stringstream";
  stringstream ss(sentence);
  string word;
  int count = 0;
  while (ss >> word) {
    ++count;
  }
  cout << "The number of words in the sentence is: " << count << endl;
}

```
count words in a sentence.
