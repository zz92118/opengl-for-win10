# opengl-for-win10
## 记得在x64下编译运行

## 记录一下opengl 安装的心路历程 glad glfw glew freeglut

* free glut+glew（glut和glew可以直接调用了）：https://developer.aliyun.com/article/791142

* 类似的方法安装glfw https://www.cnblogs.com/gamer610/p/16803642.html

* glad https://blog.csdn.net/qq_33957603/article/details/123512334

按照上述方法将所有的文件添加、复制之后，再在项目里进行如下操作：

1. 在项目属性中选择C/C++ -> 预处理器 -> 预处理器定义 NDEBUG必须添加到Debug模式中。



2. 编辑"附加依赖项"， 将  "freeglut.lib;glew32.lib;glfw3.lib;OpenGL32.lib;"复制进去，

3. 在项目属性 ----> C/C++ —> 附加包含目录 —> your_path\glad\include

4. debug模式选择x64 

LINK1104 error 的解决方法 http://t.zoukankan.com/esCharacter-p-8808727.html


## 再补一下games101环境配置

### eigen的安装
https://blog.csdn.net/wilsonass/article/details/90754525

选择C/C++  -》常规  -》  包含目录 

目录地址: cmake过后eigine的地址（好像不用make 原地址就行了） D:\eigen-3.4.0;%(AdditionalIncludeDirectories)

### opencv

https://blog.csdn.net/m0_47854694/article/details/115261082


操作完之后：

* VC++目录 包含目录 D:\opencv\build\include\opencv2;D:\opencv\build\include;$(IncludePath)�
* 库目录 D:\opencv\build\x64\vc15\lib�
* 附加依赖项 opencv_world460d.lib 

## QT 安装

* 这个没怎么记录 就是安装qt，然后下载一个插件可以在vs使用，也可以更改成x64编译格式

# Reference

* https://developer.aliyun.com/article/791142
* https://www.cnblogs.com/gamer610/p/16803642.html
* https://blog.csdn.net/qq_33957603/article/details/123512334
* http://t.zoukankan.com/esCharacter-p-8808727.html
