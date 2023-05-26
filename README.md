# 供任何脚本使用的底层工具库[core-kit]

#### How To Use
```
pip install pycorekit
```

```python
from pycorekit.ShellKit import ShellKit

# 填写IP,用户名及密码
data= ShellKit('192.168.0.1','user','123456')
# 进行连接
data.connect()

#一串待执行的命令
cmds = ["ls","ls -al"]
#模拟调用 
# autoExit 执行完成后是否自动退出
# autoExitTime 自动退出的时间,默认是30秒 autoExit 开启才会生效
data.simulate(cmds,autoExit=True,autoExitTime=1)
```