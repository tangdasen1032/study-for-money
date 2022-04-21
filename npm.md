# npm

##### 使用npm对项目进行管理

npm init

npm init -y 

##### npm安装的软件包位置

- 默认安装在当前文件下的**node_modules文件夹**
- 安装命令使用了 **-g标志则安装在全局位置 ，npm root -g 命令获取全局下依赖的位置**

##### 使用安装的包

采用模块化导入，路径名只需要填写packageName，

##### 依赖包中的脚本

安装依赖包所携带的脚本被放在**node_modules/.bin文件夹中**

###### 执行脚本

- 在终端直接执行，如： ./node_modules/.bin/script
- npx script ，npx会自动查找脚本文件，先找本地，本地没有再找全局

##### package.json

- script

可以通过**npm run scriptName 执行其对应的脚本命令**

- dependencies

项目运行时所依赖的所有安装包，安装的依赖默认放在该属性下

- devDependencies

开发时锁依赖的包，安装依赖时通过 -D 指定其为开发时所依赖的包

##### package-lock.json

在package.json中依赖包的版本

- ~1.1.1 指项目所依赖包可升级为补丁版本
- ^1.1.1指项目所依赖的包可升级为补丁版本或大版本
- 1.1.1指项目所依赖包使用指定版本

而package-lock.json则跟踪项目依赖包的确切版本

使用 npm i 安装依赖包时，会下载package-lock.json中的指定版本

##### npm常用的命令

- npm init | npm init -y
- npm i packageName@version 安装指定版本的依赖
- npm i packageName | npm install packageName

下载修饰标识

-D 开发是依赖

-g 全局安装依赖

- npm list | npm list -g	查看所安装的所有依赖包
- npm view packageName version 查看当前依赖的最新版本

##### yarn

包管理器,常用命令见官网 [go](https://www.yarnpkg.cn/getting-started/usage)
