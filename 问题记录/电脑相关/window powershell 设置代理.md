### windows powershell设置永久代理

在环境变量中增加如下环境变量
	- 变量名：**HTTP_PROXY**, 变量值 **http://localhost:7890**, *注：端口号是vpn里的端口号*
	- 变量名：**HTTPS_PROXY**, 变量值**https://localhost:7890**

### 删除永久代理

删除环境变量即可
