# 安装

输入 `npm install gitbook-cli -g` 进行安装

# 运行程序

输入 `gitbook init` 初始化项目

输入 `gitbook serve` 本地运行该项目。该方法运行的程序支持热部署，也就是当文件修改时页面可以感知到变化然后立即刷新。这种模式已然成为了前端开发或相关技术的标配。

# 目录说明

查看 SUMMARY.md 文件，在运行`gitbook init`命令的时候会按照这里的目录结构对应的模板文件。这个命令适用于新建项目初始化时或已经对目录有了一个清晰的结构的时候比较适用。如果目录需要经常调整的话，使用起来并不太方便。因为它只是生成一个seketon并不能把原来已经写好的一部分文字也转移过去。
```markdown
# Summary

* [Introduction](README.md)
* [安装](01init/README.md)
* [Chapter2](chapter2/README.md)
```

# 关于命令的一些思考

文件名最好不要使用中文，避免在部署或编译的时候由于工具或系统没有对中文进行优化而产生一些奇怪的问题。

