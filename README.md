[![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg)](https://github.com/996icu/996.ICU/blob/master/LICENSE)
[![LICENSE](https://camo.githubusercontent.com/f969af70fa6573766a11cb0a968fc82b069298f1/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f6c697a68696368616f2f6f6e652e737667)](https://github.com/eguid/vlpr4j/blob/master/LICENSE)
 # vlpr4j
基于opencv的java车牌检测识别库（支持linux、windows、mac、Android平台），识别准确率79.7%以上。 
## 基于
1、vlpr4j基于EasyPR二次开发
1、解决EasyPR的Java版本的无法编译、无法使用、opencv版本过老的问题。
## 构建
1、vlpr4j基于jdk1.7构建
2、vlpr4j基于javacpp-presets-1.3.0版本(opencv3.2.0版本)构建
## 支持
1、vlpr4j支持opencv的Mat及图片文件路径加载图像
## 使用
### 1、使用本地图片文件进行操作
 String imgPath = "res/image/test_image/plate_judge.jpg"; 
 Mat src = opencv_imgcodecs.imread(imgPath); 
 String ret=plateRecognise(src); //得到结果
 System.err.println(ret);
### 2、使用Mat进行操作 
 String ret=plateRecognise(Mat mat);  
 System.err.println(ret);
### 依赖关系
1、本项目依赖于opencv3.2.0及javacpp-1.3
2、本项目默认导入四个系统环境jar包，如有不需要的系统环境可以直接从libs中删除对应jar包即可


