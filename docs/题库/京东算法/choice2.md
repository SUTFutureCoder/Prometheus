# 选择题2
```
#include<studio.h>
class CFather
{
public:
    CFather(){}
    virtual ~CFather(){}

    void FuncA()
    {
        printf("CFather FuncA\n");
        FuncB();
    }
    virtual void FuncB()
    {
        printf("CFather FuncB\n");
    }
};
class CChild:public CFather
{
public:
    CChild(){}
    virtual ~CChild(){}

    void FuncA()
    {
        printf("CChild FuncA\n");
        FuncB();
    }
    virtual void FuncB()
    {
        printf("CChild FuncB\n");
    }
};
int main(int argc,char *argv[])
{
    CChild *child = new CChild();
    child->FuncA();

    CFather *father = static_cast<CFather *>(child);
    father->FuncA();
    return 0;
}
```
程序输出的内容是？





 > **A项** </br>CFather FuncA</br>
         CChild FuncB</br>
         CFather FuncA</br>
         CFather FuncB

 > **B项** </br>CFather FuncA</br>
         CChild FuncB</br>
         CFather FuncA</br>
         CChild FuncB

 > **C项** </br>CChild FuncA</br>
         CChild FuncB</br>
         CFather FuncA</br>
         CChild FuncB
         
 > **D项** </br>CChild FuncA</br>
         CChild FuncB</br>
         CFather FuncA</br>
         CFather FuncB