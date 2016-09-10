# Sharetribe 笔记
Sharetribe 是这个 https://www.sharetribe.com/   
开源代码的地址是这里： https://github.com/sharetribe/sharetribe   
以下是学习这个开源平台做的笔记     

<br/>
## 时间
这个笔记从 2016 年 9 月 10 号开始记录起。  
当前 Sharetribe 版本 5.11.0 （根目录下有个文件叫做 VERSION，里面只有一行文字，就是版本号）  
笔记当然是基于这个版本，所以如果你发现这里写的笔记和代码不一样，以官方代码为准。

<br/>
## 什么是 Sharetribe
https://www.sharetribe.com/   
这是个买卖的平台， 
但是和淘宝之类的不一样, 代码开源，MIT 协议，就是说拿代码去商用和闭源是 OK 的。    

<br/>
## 公司信息

<br/>
## 基于 Sharetribe 的网站有（不完全列表）    
https://www.drivevinty.com/     
https://www.cyclelifehq.com/     
https://www.foodforage.com.au/    


<br/>
## Tech Stack 技术栈
官方的 readme 里简单说了安装，配置，和一些基本的依赖。  
没列清楚技术栈。所以我一边看代码学习一边列技术栈  

Ruby 2.3.1  
Ruby on Rails 4.2.7  
Gem: Devise(做邮箱登录), Omniauth-facebook(做 Facebook 登录)  
MySQL  

服务器：不清楚，可能是 AWS  
图片托管：不清楚，可能是 CloudFront  


<br/>
## Model
用户的 Model 是 person. 并没有 account 或者 user 这样的 model



<br/>
## 小备注
Sharetribe 以前的名字叫做 Kassi，这就是为什么你在 routes.rb 里看到 Kassi 了。  
https://github.com/sizzlelab/kassi  


