# 选择题13
## 分析下面程序的编译结果。
#include<iostream.h><br>
template<class T><br>
void f1(T *t){cout<<"*t="<<"*t"<<endl;}<br>
template<class T><br>
void f1(T *t){cout<<"*t="<<t<<endl;}<br>
void main(){<br>
int i=3;<br>
f1(i);  //A<br>
f1(&i);  //B<br>
}


</br>


### **A** 程序编译没有错误。
### **B** 第二个函数模板有错
### **C** A行有错
### **D** B行有错