# 罗剑锋C++实战笔记
提高c++技能

安装g++编译器
```
sudo apt-get install g++
```

```c++
//Copyright 2022  yanqing
#include <string>
using namespace std;
#define MAX_PATH_LEN 	256	 //   常量，全大写
int g_sys_flag;		 //	 全局变量，加g_前缀
namespace linux_sys {	 //	 名字空间，全小写
	void get_rlimit_core();	  //	 函数，全小写
}
class FilePath final	 //	 类名，首字母大写
{
public:
	void set_path(const string& str);	 // 函数，全小写
private:
	string m_path;	 //	 成员变量，m_前缀

};


int main() {
  printf("hellworld\n");
  return 0;
}


```

编译
```
g++ -std=c++11 test.cpp -o a.out; ./a.out
```
