@[TOC](GO语言学习笔记)

# Go语言学习笔记

本教程适合有其他编程语言基础的人学习。教程所有内容都是个人（本人）学习时编辑整理的，内容主要是go语言基础知识和自己学习过程中对go语言的理解。文章从一个go语言初学者的角度出发，以一个go语言初学者的视角来表述知识点，让所有初学者更容易接受和理解。

## 1、入门

### 1.1 安装Go语言

我们可以通过访问[go语言中文网](<https://studygolang.com/dl>)来下载go，我们只需要下载与自己操作系统对应的Go语言安装包即可，下载完成后运行程序执行安装。图1.1.1为go语言安装包下载页面：

![1557477707330](C:\Users\Administrator\Desktop\books\go\笔记\images\1557477707330.png)

<center>图1.1.1</center>

当程序安装完成后，进入控制台（command）界面，执行命令查看系统环境变量，命令如下：

windows：

```shell
> echo %PATH%
```

mac/linux：

```shell
$ echo $PATH
```

执行上面的命令，如果打印出的内容包含你的`go安装路径/bin`，那么go语言环境就安装成功了。

如果你还不确定go语言程序是否安装成功，你也可以执行`go version`查看go环境，当出现如下类似结果即表示go语言环境安装成功。

```shell
> go version
go version go1.12.4 windows/amd64
```

### 1.2  hello world程序

下面来感受一个go语言入门示例，我们任一一目录新建一个文件`main.go`，并键入如下所示所示内容：

```go
package main

import "fmt"

func main() {
	fmt.Printf("Hello world!")
}
```

我们在当前文件（main.go）所在目录下执行`go run main.go`命令：

```shell
$ go run main.go
Hello world!
```

如果出现***Hello world!***打印在控制台就说明程序执行成功了！

下面对程序作一个详细的解释：

* 文件名main.go

  所有go程序的文件名都是以`.go`结尾的。

* package main

  指定当前go文件（程序或代码）所在包。包有点类似于`文件夹`的概念，比如main.go文件在main包下，可以理解为main.go在main文件夹下（只是类比，但实际上并不是这样的）。包也有类似于`归类`的概念，也即main.go归类在main包下。所有go程序的入口（可执行）程序都是在`main`包下的。

* import "fmt"

  import用来导包，上面所示表示导入`fmt`包，导包后，我们可以在程序中使用导入的包中定义的内容（方法、变量等等），比如`fmt.Print()`就是使用`fmt`包中的Print()函数。

* func main() {

  主函数，程序入口，也叫入口函数，一个可执行程序必须包含一个主函数，注意主函数没有参数和返回值（什么是参数和返回值？后文介绍，这里只需要知道主函数像这样写就可以了）。

* fmt.Printf("Hello world!")

  调用`fmt`包中的`Printf()`函数，在控制台打印***Hello World!***。

## 2、程序结构

## 3、基本数据类型

## 4、复合数据类型

## 5、函数

## 6、方法

## 7、接口

## 8、Goroutine和通道

## 9、共享变量及并发

## 10、包和go工具

## 11、测试

## 12、反射

## 13、底层编程







