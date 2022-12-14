## 常见问题解答

一些常见的问题都列举在这里了，希望对你有帮助。 

### 更新时窗口无响应卡死或者内容丢失

`影响范围`：客户端全版本

`问题原因`：目前未知

`解决方法`：在配置文件里把主题禁用即可`disable-theme: true`

### 连接中断

`影响范围`：客户端全版本

`问题原因`：由于网络原因，已建立的TCP连接被意外断开。俗话叫网络不稳定

`解决方法`：这不是程序bug，请检查客户端与服务器之间的网络是否流畅

### 连接被拒绝

`影响范围`：客户端全版本

`问题原因`：由于网络原因，服务器拒绝了客户端的TCP请求。俗话叫端口不通

`解决方法`：这不是程序bug，请排查与服务器直接的网络是否通常，是否需要放开安全组规则，配置端口映射，放行服务器防火墙规则，也请检查客户端配置文件中的地址是否填写错误等

### 连接超时

`影响范围`：客户端全版本

`问题原因`：由于网络原因，服务器未能在指定时间内及时应答客户端的TCP数据包。可能是网络不稳定也可能端口不通

`解决方法`：这不是程序bug，请检查客户端与服务器之间的网络是否稳定

### 配置文件中的选项(xxx)无效

`影响范围`：客户端全版本

`问题原因`：配置文件`config.yml`中找不到名为xxx的配置项，或者配置项的数据类型不正确

`解决方法`：删除配置文件并重新从文件内部解压重新配置一次

### xxx无法解码为xxx格式

`影响范围`：客户端全版本

`问题原因`：对应的数据无法解析到对应的格式，比如json格式或者yaml格式

`可能的情况和解决办法：`：

+ `v-xxx.json`无法解码为`版本记录文件`格式：向我报告此问题

### Http状态码(xxx)不在2xx-3xx之间

`影响范围`：客户端全版本

`问题原因`：访问对应URL时，服务端返回了一个表示错误的HTTP状态码（即不在2xx-3xx之间）

`解决方法`：向我报告此问题#HTTP状态码不正确)

### 找不到.minecraft目录

即使把Jar客户端放到`.minecraft`目录旁也提示找不到的问题

`影响范围`：Jar客户端全版本

`问题原因`：启动Jar文件时，在`打开方式`中选择了以Java启动打开，而非默认Java启动

`解决方案`：将Jar文件设置为默认使用Java运行，然后使用双击方式启动

