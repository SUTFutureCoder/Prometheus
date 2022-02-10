# 选择题8
## 假定c是一个string的multiset,v是一个string的vector,解释下面的调用，指出哪个调用是不合法的：


</br>

### **A** copy(v.begin(),v.end(),back_inserter(c));
### **B** copy(c.begin(),c.end(),inserter(v,v.end()));
### **C** copy(c.begin(),c.end(),back_inserter(v));
### **D** copy(v.begin(),v.end(),inserter(c,c.end()));