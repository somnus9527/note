### windows powershell设置永久代理

在环境变量中增加如下环境变量
	- 变量名：**HTTP_PROXY**, 变量值 **http://localhost:7890**, *注：端口号是vpn里的端口号*
	- 变量名：**HTTPS_PROXY**, 变量值**https://localhost:7890**

### 删除永久代理

删除环境变量即可



**发现上述操作不一定生效，可以以管理员身份打开powershell然后设置： ```netsh winhttp set proxy 127.0.0.1:58591```, 端口改成实际端口**， 可以用过```netsh winhttp show proxy```查看是否已经设置代理， 通过```Invoke-WebRequest http://www.example.com/```查看代理是否设置成功， 可以使用```netsh winhttp reset proxy```取消设置的代理

