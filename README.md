#  nginxWebUI runCmd RCE漏洞 POC
nginxWebUI是一款图形化管理nginx配置的工具，能通过网页快速配置nginx的各种功能。
nginxWebUI后台提供执行nginx相关命令的接口，由于未对用户的输入进行过滤，导致可在后台执行任意命令。并且该系统权限校验存在问题，导致存在权限绕过，在前台可直接调用后台接口，最终可以达到无条件远程命令执行的效果。
```
Usage:
  python3  SMART-PARK.py -h
```
![示例](https://github.com/gallopsec/nginxWebUI/blob/main/poc.png)
![示例](https://github.com/gallopsec/nginxWebUI/blob/main/test.png)
