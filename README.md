## 如何创建一个属于自己的模块，并在其他项目中引用

1. 创建一个项目

2. go mod init 模块名
这里我的模块名为github.com/elpsyr/go_module_demo


3. 给这个项目有新建一个go文件，并在里面写一个对外暴露的方法
```go
func Say() string{
	return "Hello ,I'm module v1"
}
```

4. 这时候已经差不多完成了
我们还需要为这个模块指定一下版本，将代码上传至github后，给项目加个tag，也就是版本号