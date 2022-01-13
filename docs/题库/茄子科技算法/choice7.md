# 选择题7
## 以下函数的时间复杂度和空间复杂度为（）
int Function(int n){</br>
    if(n<=2)</br>
        return n;</br>
    else
        return Function(n-1)+Function(n-2);</br>
}
### **A** T(n)=O(2<sup>n</sup>),S(n)= O(1)
### **B** T(n)=O(1),S(n)= O(1)
### **C** T(n)=O(2<sup>n</sup>),S(n)= O(n)
### **D** T(n)=O(n),S(n)= O(n)