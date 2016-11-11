# a51m

> 该工具目前仅适用于i.MX6 Android 5.1.1源代码，未测试其他版本是否可用。

当我们单独生成U-Boot、boot.img、system.img的时候，并不需要去按照Android那套流程走，因为那样耗费的时间太长了，经常要等很久，耗不起，跟踪了android输出信息：[I.MX6 Android 5.1 快速合成系统](http://www.cnblogs.com/zengjfgit/p/6052084.html)，于是编写了这个快速合成对应部分内容工具，具有如下功能：

  * 编译U-Boot；
  * 编译内核，合成ramdisk.img，进而合成boot.img；
  * 合成system.img

源代码是shell脚本，请尽量自己阅读，看其中怎么工作的，并修改成符合自己要求的版本。

## 使用方法

```Shell
    a51m <ub | bi | fs> 
        1. ub: U-Boot compile.
        2. bi: boot.img compile.
        3. fs: system.img repack
```
