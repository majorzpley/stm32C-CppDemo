# stm32C-CppDemo
对于C/C++混合编程的一些tips，我在b站这个链接:https://www.bilibili.com/read/cv20304058/
看到了一些C/C++混合编译的教程，通过我自己的实践发现一些问题并解决

1、开发环境:
    -代码生成器:stm32cubemxHal库，测试使用的是apme103和stm32f103rct6以及stm32f103c8t6均可以按此方法使用;
    -编译器：arm gnu toolchain，网站是这个z;https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads
    -编辑器和调试环境:vscode，这个可以找找教程吧，我就不赘述了
2、步骤
    -首先使用cubemx生成带Makefile的项目;
    -其次修改Makefile，可以参照我之前fft的源码，里面有s汇编文件、lib文件和S文件等说明，需要有一定的Makefile语法能力，目前我正在修改Makefile的使用
    -最后在vscode中调试，可以参照源码中的cpp_xxx.json和task.json以及launch.json来做修改
    