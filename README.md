## 右键执行npm项目中的脚本

### 运行环境
- Windows系统
- PowerShell 3.0+

### 文件说明
- [package.ps1](./package.ps1): PowerShell脚本文件, 读取并解析npm项目入口文件package.json(如果存在的话), 并将scripts配置项中的命令列出, 供使用者选择, **选择完毕回车即可执行命令**.   
- [package.reg](./package.reg): 注册表脚本文件, 将[package.ps1](./package.ps1)脚本文件注册到右键菜单.

### 使用说明
在第一次使用之前, 需要先注册右键菜单项, 注册过之后, 后面再使用的话, 只需要在右键选择菜单项: 执行NPM脚本, 具体步骤请参考: 
#### 注册右键菜单项
1. 将文件保存到本地.
2. 在package.reg文件里, 修改一下package.ps1文件的路径, 保存.
3. 运行package.reg文件.

#### 执行NPM脚本
1. 在包含有package.json文件的项目的根目录中, 选择右键菜单项: 执行NPM脚本.
2. 选择要执行的命令, 然后回车.

### 注意事项
- package.ps1文件的编码格式为GBK.
- package.reg文件里需要用到 package.ps1文件 所在的本地路径.