# AdHoc TurnServer
  这是一个使用C++语言编写的中转服务器！
  
## 目录说明
- [net](net) 
	与网络通信通信相关的文件。
- [tars-patch](tars-patch)
	tars框架部分补丁文件
	
## 使用说明

-运行依赖
	
	1.Protobuf,Protobuf安装在服务器上面并配置好运行环境变量,
	2.rapidjson,rapidjosn放在tars 源码的 /Tars/cpp/thirdparty 目录下即可

-编译步骤
	
	1.首先编译下载的Tars源码(编译CPP开发部分即可)
	2.根据补丁文件修改Tars源码,由于Tars近期开源且处于更新中因此采用命令打补丁可能会失败，建议手动修改
	3.重新编译修改后的Tars源码(或者先修改Tars源码然后再编译可以只编译一遍)
	4.重新编译之后要执行安装命令：Tars/cpp/build/build.sh install
	5.编译中转服务器代码,在当前目录下执行 make 命令即可



