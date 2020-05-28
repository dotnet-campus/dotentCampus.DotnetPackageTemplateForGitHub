# dotnetCampus.DotnetPackageTemplateForGitHub

dotnet campus .NET Package Template for GitHub

提供通用 CBB 底层库项目创建模板

使用此模板创建将可以

1. 自动接入 CI 测试
1. 自动接入 Tag 打包和合并 master 打包
1. 符合规范的文件结构

## 使用方法

命令行输入下面代码安装

```csharp
dotnet new -i dotentCampus.DotnetPackageTemplateForGitHub
```

之后创建项目可采用下面代码创建

```csharp
dotnet new githubcbb -o 项目文件夹
```

更多请看 [创建 dotnet new 项模板 - .NET Core CLI - .NET Core](https://docs.microsoft.com/zh-cn/dotnet/core/tutorials/cli-templates-create-item-template )

默认使用 Tag 打包方法，也就是使用 git 添加一个 Tag 推送上去将会自动解析这个 Tag 版本号打包推送

推荐更改 Directory.Build.props 的作者名等信息