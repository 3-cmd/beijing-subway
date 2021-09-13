# 北京地铁预约出行 - 定时预约系统

#### 介绍

每天早上九点会检查第二天是否为工作日  
如果为工作日中午十二点自动进行预约操作  
access_token有效期大概在一周
由于官网的刷新token接口不对，只能检查token有效期进行提醒   
获取token方法（建议使用google）：登录pc端抢票系统f12切换为手机模式https://webui.mybti.cn     
控制台内输入: localStorage["yycx-a-token"]

#### 使用

##### 1.修改预约站点
默认抢票点为：昌平线-沙河站
可以在TaskMetro.java中进行修改

##### 2.修改抢票时间段及个人账号access_token
打开application.properties
对应修改即可，注意格式
##### 3.修改推送邮件（建议使用qq邮箱）
打开mail.setting  
修改from和pass配置项        
注意密码需要使用smtp密码,获取方法：（qq邮箱）     
https://jingyan.baidu.com/article/6079ad0eb14aaa28fe86db5a.html

##### 4.执行
