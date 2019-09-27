# AnsiblePlaybook
存放常用playbook

1, preOraInst目录存放在redhat linux 7以上的版本中安装oracle 11g,12c,18c,19c的准备工作 ,提升了管理员部署的效率   
  
  A, 下载 preOraInst目录到ansible所在的服务器上,软件介质可以存放preOraInst/files目录下一起复制到目标服务器;  
  B, 修改preOraInst/main.yml相关具体内容，比如oracle_home,oracle_sid,OS的信息等;  
  C, 调用方式   ansible-playbook main.yml  -i /tmp/hosts  
  D, 执行完成后，需要重启操作系统以使用配置生效;   

2, postOra19CInst目录存放在redhat linux 7以上的版本中安装oracle 19c的软件安装 ,提升了管理员部署的效率   
  
  A, 下载 postOra19CInst目录到ansible所在的服务器上,软件介质可以存放postOra19CInst/files目录下一起复制到目标服务器;  
  B, 修改 postOra19CInst/mail.yml相关具体内容，比如oracle_home,oracle_sid的信息等;  
  C, 调用方式   ansible-playbook main.yml  -i /tmp/hosts  

3, create19CDb目录存放的redhat linux 7中创建oracle 19c NonCDB模式的数据库;
  
  A, 下载 create19CDb目录到ansible所在的服务器上,软件介质可以存放postOra19CInst/files目录下一起复制到目标服务器;  
  B, 修改 create19CDb/main.yml相关具体内容，比如oracle_home,oracle_sid,sys_system_pwd的信息等;  
  C, 调用方式   ansible-playbook main.yml  -i /tmp/hosts  ;

