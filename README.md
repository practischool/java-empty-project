# 简介

科蚪实务学堂Java入门课程的空白项目，用于帮助各位助教上手，了解如何在IntelliJ里面运行一个本课程的相关代码。

# 用法

1. 先修内容：没用过IntelliJ的童鞋，可能需要熟悉一下如何使用IDE。
2. 通过IntelliJ克隆本代码仓库。（也可通过命令行克隆，然后在IntelliJ里面打开。）
3. 在`src`目录下新建一个`HelloKarel.Java`文件，将如下内容复制粘贴进去，运行后即可看到效果。
    ```java
    import stanford.karel.Karel;
    
    public class HelloKarel extends Karel {
        public void run() {
            // 让Karel向前移动一步
            move();
    
            // 左转
            turnLeft();
    
            // 向前移动两步
            move();
            move();
        }
    }
    ```
4. 在`src`目录下新建一个`HelloGraphicsProgram.Java`文件，将如下内容复制粘贴进去，运行后即可看到效果。
    ```java
    import acm.graphics.GLabel;
    import acm.program.GraphicsProgram;
    
    public class HelloGraphicsProgram extends GraphicsProgram {
        public void run() {
            // 新建一个label
            GLabel l = new GLabel("Hello Graphics Program :)");
    
            // 添加到canvas上面(100, 100)的位置
            add(l, 100, 100);
        }
    }
    ```
5. 在`src`目录下新建一个`HelloConsoleProgram.Java`文件，将如下内容复制粘贴进去，运行后即可看到效果。
    ```java
    import acm.program.ConsoleProgram;
    
    public class HelloConsoleProgram extends ConsoleProgram {
        public void run() {
            println("Hello Console Program:)");
        }
    }
    ```
6. 自行创建文件，进行编程。

# 原理

1. 主要基于斯坦福CS106A课程公开材料制作
2. 所用到的包被编译进了`lib/spl.jar`中
3. 除直接阅读`spl.jar`代码外，也可以在斯坦福网站找到相关的英文文档。