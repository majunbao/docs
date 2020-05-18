# YARN
前端代码的包管理器。

## 常用命令

- yarn init                初始化新项目
- yarn add                 添加到dependencies依赖类别
- yarn add --dev           添加到devDependencies类别
- yarn add --peer          添加到peerDependencies类别
- yarn add --optional      添加到optionalDependencies类别
- yarn upgrade             升级依赖
- yarn remove              移除依赖
- yarn install OR yarn     安装项目的全部依赖
- yarn info [package@version]

- (英文网站)[https://classic.yarnpkg.com/en/]
- (中文网站)[https://classic.yarnpkg.com/zh-Hans/]

## 依赖类型

依赖关系可用于许多不同目的。构想项目需要一些依赖关系，而运行程序时也需要其他依赖关系。因此，您可以拥有许多不同类型的依赖项（例如：`dependencies`， `devDependencies`， and `peerDependencies` ）。

### dependencies
这些是你的常规依赖项，或者是运行代码所需要的依赖项（例如 `React` 或 `ImmutableJS`）。

### devDependencies
这些是你的开发依赖项。在开发工作流中某些时候需要的依赖关系，而不是在运行代码时需要的依赖关系（例如 `Bable` 或 `Flow`）。

### peerDependencies
`Peer` 依赖是一种特殊类型的依赖项，只有在发布自己的程序包时才会出现。
具有 `Peer` 依赖意味着，你的软件包和安装软件包的人具有完全相同的依赖性。这对于像 `React` 这样的程序包很有用，因为它们需要一个单独的 `react-dom` 副本，安装者也需要使用它。

### optionalDependencies
可选的依赖关系就是：optional。如果它们无法安装。Yarn 仍然会说安装过程成功。
这对于不一定在每台机器上都起作用的依赖项很有用，并且如果没有安装依赖项，则您有一个备用计划（例如 `Watchman`）。

### bundledDependencies
发布软件包时将捆绑在一起的软件包名称数组。
捆绑的依赖项应位于项目内部。该功能基本上与 `dependencies` 相同。当运行 `yarn pack` 它们也将被打包。
通常从 npm 注册表中安装常规依赖项。如果正常的依赖关系不行，则捆绑的依赖关系很有用：

- 当你想重新使用不是来自 npm 注册表或者已被修改的第三方库时。
- 当你想将自己的项目重新做模块时。
- 当你想使用模块分发一些文件时。