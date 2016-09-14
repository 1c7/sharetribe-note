# Sharetribe Note 
Sharetribe is this: https://www.sharetribe.com/   
Open source code is here： https://github.com/sharetribe/sharetribe   

Below are note I take when I am learning how sharetribe work.

File beside `readme.md` you don't have to look inside, because these are unfinished note.  
I would put link down below once it finished, so you don't have to worry about it.  

<br/>
## Sharetribe Version (5.11)
(2016/Septmber/14) Sharetribe Version is 5.11   
All these note down below are base on 5.11  
if you find any inconsistent between Sharetribe Code and This note, Code is always right.

<br/>
## What is Sharetribe?
https://www.sharetribe.com/   
A platform 
但是和淘宝之类的不一样, 代码开源，MIT 协议，就是说拿代码去商用和闭源是 OK 的。   

<br/>
## How to pay?(on Sharetribe)
Paypal    


<br/>
## Short description about company
Company locate at [Helsinki, Finland](https://www.google.com/maps/place/Helsinki,+Finland/@58.7019284,16.6558103,4.79z/data=!4m5!3m4!1s0x46920bc796210691:0xcd4ebd843be2f763!8m2!3d60.1698557!4d24.938379)   
芬兰语是主要语言  
[Team](https://www.sharetribe.com/team.html)  - 15个人，全是男的


<br/>
## Website that base on Sharetribe
http://www.studiotime.io/  - 按天/小时租用音乐工作室  
https://www.drivevinty.com/     
https://www.cyclelifehq.com/     
https://www.foodforage.com.au/    

Reference: 


<br/>
## Tech Stack
- Ruby 2.3.1  
- Ruby on Rails 4.2.7  

- MySQL  
- Editor is using Mercury  
- Deploy: custom script (not using Mina or Cap3)  
- Server: Heroku (BaaS)  
- Image: Amazon S3  
- Gem: Devise(for Email/Username Signup/Login), 
    Omniauth-facebook(做 Facebook 登录)  


<br/>
## Model

- Model for store user info is `person` (Table name is `people`) (app/models/person.rb)
  not using any model name(`user` or `account`)


## Controller



<br/>
### 小备注
Sharetribe 以前的名字叫做 Kassi，这就是为什么你在 routes.rb 里看到 Kassi 了。  
https://github.com/sizzlelab/kassi  


