# 右键执行npm项目中的脚本

## 运行环境
- Windows系统
- PowerShell 3.0+

## 使用说明
[package.ps1](./package.ps1)脚本文件: 读取并解析npm项目入口文件package.json(如果存在的话), 并将scripts配置项中的命令列出, 供使用者选择, **选择完毕回车即可执行命令**. 
[package.reg](./package.reg)注册表脚本文件: 将[package.ps1](./package.ps1)脚本文件注册到右键菜单

## 注意事项
- package.ps1文件的编码格式为GBK
- package.reg文件里需要用到 package.ps1文件 所在的本地路径