# 类型信息

1. Java 类都是在第一次使用时才被加载的，当程序创建第一个对类的静态成员的引用时就会加载这个类。因此说明构造器也是类静态方法。

类加载流程：

1. 加载：默认的类加载器根据类名查找 .class 文件。从校验过的字节码中创建一个 Class 的对象。

2. 链接：校验：字节码被加载时会接受验证，以确保其没有配破坏，并且不包含不良 Java 代码（安全防范的措施之一）。为静态域分配存储空间，并且有必要的话，将解析这个类创建的对其它类的又有引用。

3. 初始化：如果类具有超类，则对其初始化，执行静态初始化器和初始化快。



