Java特性:

1. 面向对象（封装，继承，多态）
2. 平台无关性（JVM运行.class文件）
3. 语言（泛型，Lambda）
4. 类库（集合，并发，网络，IO/NIO）
5. JRE（Java运行环境，JVM，类库）
6. JDK（Java开发工具，包括JRE，javac，诊断工具）

Java是解析运行吗？

不正确！

1，Java源代码经过Javac编译成.class文件

2，.class文件经JVM解析或编译运行。

（1）解析:.class文件经过JVM内嵌的解析器解析执行。

（2）编译:存在JIT编译器（Just In Time Compile 即时编译器）把经常运行的代码作为"热点

代码"编译与本地平台相关的机器码，并进行各种层次的优化。

（3）AOT编译器: Java 9提供的直接将所有代码编译成机器码执行。



