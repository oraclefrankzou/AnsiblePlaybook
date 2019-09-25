# AnsiblePlaybook
存放常用playbook

1, preOraInst目录存放在redhat linux 7以上的版本中安装oracle 11g,12c,18c,19c的准备工作
  A, 下载 preOraInst目录到ansible所在的服务器上;
  B, 修改mail.yml相关具体内容，比如oracle_home,oracle_sid,OS的信息等;
  C, 调用方式   ansible-playbook main.yml  -i /tmp/hosts
