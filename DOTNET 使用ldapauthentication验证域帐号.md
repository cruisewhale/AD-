1. 碰到无法验证的事件  
  1）之前项目一直正常, 域帐号也能在webservice中正常通过 LADPAUTHENCATION 方法验证. 但有一天突然无法验证. 系统管理员发现服务器在安装补丁, 重新启动后能过一会后恢复正常  
  2) 过几天后, 情况又在出现, 重新启动服务器仍无法恢复     
  3) 经过排查, 仍无法确定原因. 后发现同样的程序在程序员的电脑上上能正常运行, 于是在将验证域指向另一个域, 发现程序能正常运行     
  4) 发现在故障服务器上和程序员的电脑上PING 相同的域名返回不同的IP地址.   
  5) 运行环境有两台域控服务器, 其中一台可以有域名进行验证,另一台只能用IP验证.   
  6) 将程序的验证服务器改为IP地址, 重新测试恢复正常.
  
