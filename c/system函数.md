# system  
> 包含在头文件 “stdlib.h” 中  
> int system(const char * command)  
## 函数功能  
执行 shell(Linux/Unix系统) 命令，参数字符串command为命令名。  
说明：在Linux/Unix系统中，system函数会调用fork函数产生子进程，由子进程来执行command命令，命令执行完后随即返回原调用的进程。  

## 函数返回值  
命令执行成功返回0，执行失败返回-1。  
## 示例
> system("modprobe lockd");  
