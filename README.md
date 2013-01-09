# 说明

可执行文件为Release目录下面Radiosity.exe

## 运行参数

    Radiosity.exe
    
    --help      : show help information
    --area      : The Area of Triangle[Default Value : 0.001]
    --file      : Obj file name[Necessary]
    --shot      : Save ScreenShot[Default Value : false]

*   area参数为每个剖分后三角形的面积大小.场景被导入到程序后，所有的大小都被归一化后[-1.0, 1.0]之间

*   file只支持obj文件读入，一定要附带mtl文件，其中mtl中叫做light的项目被认为是光源。

## 默认的调用脚本

*   areaHigh.bat:
Radiosity.exe --file=cornell_box.obj --area=0.1

*   areaMiddle.bat:
Radiosity.exe --file=cornell_box.obj --area=0.01

*   areaSmall.bat:
Radiosity.exe --file=cornell_box.obj --area=0.001

其中area越小，三角形越多，效果越好，速度越慢。

## 操作说明

   *    按键1    GL_POINTS显示 
   *    按键2    GL_LINES显示
   *    按键3    GL_TRIANGES显示
   *    按键w    fovy减小
   *    按键s    fovy变大
   *    按键p    截图

## 编程环境

   OS: win7 64位系统   
   IDE: msvc2010 
