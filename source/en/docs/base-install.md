# Installation

## Install Feflow CLI

<!-- `Feflow` 支持 Node 6.0 以上的版本，你可以使用以下命令来安装我们提供的命令行工具： -->

Feflow support Node 6.0 and above, you can use follow command to install it:

```sh
npm i feflow-cli -g
# or `yarn global add feflow-cli`
```

<!-- 如果你是第一次安装，那么需要运行一次 `Feflow` 来初始化： -->

After install, you can run `feflow` to init:

```sh
feflow
```

![Feflow初始化](https://pub.idqqimg.com/45b5f10631af4b6da8a7c81ac8eea01c.svg)

这里让你填写的 npm registry 和 npm proxy 是为了让你用 `Feflow` 安装模块的时候保证网络畅通或者是从私有仓库上下载 NPM 包。比如说你想用淘宝镜像安装模块，那么这里的 npm registry 要填写 https://registry.npm.taobao.org， 这样一来，`Feflow` 在安装模块时，就会通过这个配置进行包的下载。



如果你不小心一路回车使用了默认配置，那么你还可以通过以下命令来配置。以淘宝镜像为例：

```sh
feflow config set registry https://registry.npm.taobao.org
```

> 关于 feflow config 命令的详解可以看[这里](./base-plugins-inner.html#全局配置插件)

<!-- ## 脚手架安装 -->
## Install Scaffold

`Feflow` 的核心部分并没有一个脚手架，脚手架都是通过 `Feflow` 来安装的。为了简单起见，你可以先使用我们团队提供的脚手架 [generator-ivweb](https://github.com/feflow/generator-ivweb) 来继续这个教程。可以用如下命令安装：

Feflow core doesn't contain scaffold, you should install it via Feflow. To be simple, you can install [generator-ivweb](https://github.com/feflow/generator-ivweb) to be continue.

```sh
feflow install generator-ivweb
```

<!-- > 关于脚手架详细内容可以看[这里](./advance-scaffold-custom.html) -->

> Read [this](./advance-scaffold-custom.html) can get more informations about scaffold.

<!-- 到这里，脚手架就安装成功了，下面就可以开始创建项目了。 -->

Now, the scaffold is installed successfully, you can start creating your project.

<!-- ## 构建器安装（可选） -->
## Install Builder (optional)

`generator-ivweb` 生成的项目默认使用了 [builder-webpack4](https://github.com/feflow/builder-webpack4) 作为构建器，你可以先安装它，当然，如果你不安装，在运行 `feflow dev` 时 Feflow 会自动帮你安装上。安装命令如下：

If you used `generator-ivweb` to create project, you can install [builder-webpack4](https://github.com/feflow/builder-webpack4) as a builder, which is default builder in this project. However, if you don't install it, when you run `feflow dev`, Feflow will install it automatically.

```sh
feflow install builder-webpack4
```
