# VSCode 配置

主要配置C++、Python的ROS开发环境

## 1.VSCode的配置

主要分为全局配置和工作空间配置。全局配置存储在`.config/Code/User/settings.json`， 该文件会被自动同步到VSCode服务器。工作空间配置存储在每个工作空间中的.vscode文件夹中，这个文件夹不会自动同步。

## 2.工作空间配置

主要包含一下三个文件。只要配置c_cpp_properties.json即可，然后用CMake插件调试（Crtl + F5）。 不用去配置繁琐的launch.json和task.json. [参考1](https://www.guyuehome.com/20977)
* c_cpp_properties.json: C++配置文件
* launch.json: 启动代码调试相关的配置文件
* tasks.json: 自定义任务列表

## 3.测试用例

此目录下已经包含了普通c++工程和c++ ros工程，能运行、调试这两个工程说明配置完成了。注意，ros工程下面的.vscode/c_cpp_properties.json已经配好，能找到ros头文件，可用作模板。

* TODO: [在全局设置中设定c++默认头文件，免得每个工程配置一遍](https://blog.csdn.net/wbvalid/article/details/115001149)