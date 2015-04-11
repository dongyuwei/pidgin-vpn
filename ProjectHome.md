## 利用pidgin d-bus接口做内网穿透、远程控制 ##

for example:
  * buddyA:xxx@gmail.com;
  * buddyB:yyy@gmail.com;

### if buddyB in buddyA's trusted\_buddy\_list,when buddyA Received buddyB's Msg,buddyA can eval the python code inclued in Msg(in the form of:<%any python code%>),then send the execution result as feedback to buddyB. ###

the msg format is like this:
## <%import os; os.system('ls -l');%> ##
![http://dl.javaeye.com/upload/attachment/193147/51539c93-88a4-3c0f-ac72-8c3be2a42a8c.png](http://dl.javaeye.com/upload/attachment/193147/51539c93-88a4-3c0f-ac72-8c3be2a42a8c.png)
# In short: you can using it as using some VPN or SSH client #
### you can use one IM account(or two diffrent IM accounts) for test ###
### the first step is:modify the trusted\_buddy\_list = ["your\_IM\_account"] ###
### I tested pidgin's gtalk msn qq2008 protocal under my ubuntu. ###
