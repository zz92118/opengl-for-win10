# opengl-for-win10

## 记录一下opengl 安装的心路历程 glad glfw glew freeglut

* free glut+glew（glut和glew可以直接调用了）：https://developer.aliyun.com/article/791142

* 类似的方法安装glfw https://www.cnblogs.com/gamer610/p/16803642.html

* glad https://blog.csdn.net/qq_33957603/article/details/123512334

按照上述方法将所有的文件添加、复制之后，再在项目里进行如下操作：

1. 在项目属性中选择C/C++ -> 预处理器 -> 预处理器定义 NDEBUG必须添加到Debug模式中。

2. 编辑"附加依赖项"， 将  "freeglut.lib;glew32.lib;glfw3.lib;OpenGL32.lib;"复制进去，

3. debug模式选择x64 

LINK1104 error 的解决方法 http://t.zoukankan.com/esCharacter-p-8808727.html

# Reference

* https://developer.aliyun.com/article/791142
* https://www.cnblogs.com/gamer610/p/16803642.html
* https://blog.csdn.net/qq_33957603/article/details/123512334
* http://t.zoukankan.com/esCharacter-p-8808727.html
