[English](README.md) ∙ [简体中文](README.zh-CN.md)

# Goproxy 中国

中国最可靠的 Go 模块代理。

![39C6C4A2-AF08-4B00-915D-2FCA96767E16](https://user-images.githubusercontent.com/5037285/62007948-66cdad00-b186-11e9-899e-01ccb76951d9.jpeg)

Goproxy 中国完全实现了 Go 的[模块代理协议](https://golang.org/cmd/go/#hdr-Module_proxy_protocol)。并且它是一个由中国备受信赖的云服务提供商[七牛云](https://www.qiniu.com)支持的非营利性项目。我们的目标是为中国和世界上其他地方的 Gopher 们提供一个免费的、可靠的、持续在线的且经过 CDN 加速的模块代理。

请注意，Goproxy 中国只专注于服务在 [https://goproxy.cn](https://goproxy.cn) 的 Web 应用本身的开发。如果你正在寻找一种极其简单的方法来搭建你自己的 Go 模块代理，那么你应该看一下 [Goproxy](https://github.com/goproxy/goproxy)，Goproxy 中国就是基于它开发的。

愉快地编码吧，Gopher 们！;-)

## 功劳

* 作者：[盛傲飞](https://aofeisheng.com)
* 维护者：[盛傲飞](https://aofeisheng.com)
* 赞助商：[七牛云](https://www.qiniu.com)
* 推动者：[许式伟（七牛云的创始人兼首席执行官）](https://baike.baidu.com/item/许式伟)、陶纯堂和[茂力夫](https://github.com/forrest-mao)

## 常见问题

**问：为什么创建 Goproxy 中国？**

答：由于中国政府的网络监管系统，Go 生态系统中有着许多中国 Gopher 们无法获取的模块，比如最著名的 `golang.org/x/...`。并且在中国大陆从 GitHub 获取模块的速度也有点慢。因此，我们创建了 Goproxy 中国，使在中国的 Gopher 们能更好地使用 Go 模块。事实上，由于 [goproxy.cn](https://goproxy.cn) 已通过 CDN 加速，所以其他国家的 Gopher 们也可以使用它。

**问：使用 Goproxy 中国是否安全？**

答：当然，和所有其他的 Go 模块代理一样，我们只是将模块原封不动地缓存起来，所以我们可以向你保证它们绝对不会在我们这边被篡改。不过，如果你还是不能够完全信任我们，那么你可以使用最值得信任的校验和数据库 [sum.golang.org](https://sum.golang.org) 来确保你从我们这里获取的模块没有被篡改过，自从 Goproxy 中国已经支持了[代理校验和数据库](https://go.googlesource.com/proposal/+/master/design/25530-sumdb.md#proxying-a-checksum-database)。

**问：Goproxy 中国在中国是合法的吗？**

答：Goproxy 中国是一个由商业支持的项目而不是一个个人项目。并且它已经 ICP 备案在中华人民共和国工业和信息化部（ICP 备案号：[沪ICP备11037377号-56](http://beian.miit.gov.cn)），这也就意味着它在中国完全合法。

**问：为什么不使用 [proxy.golang.org](https://proxy.golang.org)？**

答：因为 [proxy.golang.org](https://proxy.golang.org) 在中国大陆被屏蔽了，所以，不使用。但是，如果你不在中国大陆，那么我们建议你优先考虑使用 [proxy.golang.org](https://proxy.golang.org)，毕竟它看起来更加官方。一旦你进入了中国大陆，我们希望你能在第一时间想到 [goproxy.cn](https://goproxy.cn)，这也是我们选择 `.cn` 作为域名后缀的主要原因。

## 用法

### macOS 或 Linux

打开你的终端并执行：

```bash
$ export GOPROXY=https://goproxy.cn
```

或者

```bash
$ echo "GOPROXY=https://goproxy.cn" >> ~/.profile && source ~/.profile
```

完成。

### Windows

打开你的 PowerShell 并执行：

```powershell
C:\> $env:GOPROXY = "https://goproxy.cn"
```

或者

```md
1. 打开“开始”并搜索“env”
2. 选择“编辑系统环境变量”
3. 点击“环境变量…”按钮
4. 在“<你的用户名> 的用户变量”章节下（上半部分）
5. 点击“新建…”按钮
6. 选择“变量名”输入框并输入“GOPROXY”
7. 选择“变量值”输入框并输入“https://goproxy.cn”
8. 点击“确定”按钮
```

完成。

## 社区

如果你想要参与讨论 Goproxy 中国或者询问和它相关的问题，只需要在[这里](https://github.com/goproxy/goproxy.cn/issues)发表你的问题或看法即可。

## 贡献

如果你想要帮助一起构建 Goproxy 中国，只需要简单地遵循[这个](https://github.com/goproxy/goproxy.cn/wiki/Contributing)在[这里](https://github.com/goproxy/goproxy.cn/pulls)提交你的 PR 即可。

## 许可证

该项目是基于 Unlicense 许可证发布的。

许可证可以在[这里](LICENSE)找到。
