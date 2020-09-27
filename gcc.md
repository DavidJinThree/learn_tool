# sublime gcc build
CPP 			这个会编译当前文件，并弹出一个cmd命令框（运行这个程序）
CPP-Build-Only	就是会只编译一下
CPP-Run-Only	就是只运行一下

CPP-Pipe Build and Run 会在当前代码所在目录找，找到in文件（没有后缀）的内容作为输入，并且，输出给out文件（同样没有后缀）
CPP-Pipe Run Only 跟上面的唯一区别，就是不会编译。就只输出而已。

Project Build & Run 就是将当前目录下的所有cpp文件，然后集合编译为一个文件，并且，输出为project.exe的文件，且执行该文件。
Project Build Only，只编译，不运行。
Project Run Only，只运行，不编译。