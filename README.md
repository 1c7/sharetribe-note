# Sharetribe Note 
Sharetribe is this: https://www.sharetribe.com/   
Open Source Code is here： https://github.com/sharetribe/sharetribe   

Below are note I take when I am learning how sharetribe work.

File beside `readme.md` you don't have to look inside, because these are unfinished note.  
I would put link down below once it finished, so you don't have to worry about it.  

(I am not native English speaker, if you spot any grammar error, Please point out help me improve, Thanks)

<br/>
## Sharetribe Version (5.11)
(2016/Septmber/14) Sharetribe Version is 5.11   
All these note down below are base on 5.11  
if you find any inconsistent between Sharetribe Code and This note, Code is always right.

<br/>
## What is Sharetribe?
https://www.sharetribe.com/   
[About](https://www.sharetribe.com/about.html)  
[Team](https://www.sharetribe.com/team.html)  
A Open Source Marketplace, under MIT license.   
(MIT license mean you can modify code, sell these code. only thing you have to do is keep licence file.)   

<br/>
## How to pay?(on Sharetribe)
Paypal    


<br/>
## Short description about company
Company locate at [Helsinki, Finland](https://www.google.com/maps/place/Helsinki,+Finland/@58.7019284,16.6558103,4.79z/data=!4m5!3m4!1s0x46920bc796210691:0xcd4ebd843be2f763!8m2!3d60.1698557!4d24.938379)   
people there speck Finnish 


<br/>
## Website that base on Sharetribe
http://www.studiotime.io/  - 按天/小时租用音乐工作室  
https://www.drivevinty.com/     
https://www.cyclelifehq.com/     
https://www.foodforage.com.au/    

Reference: 
[Offcial Website: Success Story](https://www.sharetribe.com/stories.html)  
[Sharetribe Community: Marketplace Showroom](https://www.sharetribe.com/community/t/marketplace-showroom-are-you-hosting-an-open-source-sharetribe-marketplace-advertise-it-here/51/1)

<br/>
## Tech Stack
- Ruby 2.3.1  
- Ruby on Rails 4.2.7  
- MySQL  
- "what you see is what you get" Editor [Mercury](http://jejacks0n.github.io/mercury/)  
- Deploy: Custom Script (not using Mina or Cap3)  
- Server: Heroku (BaaS)  
- Image: Amazon S3  
- Notable Gem: 
    -  Devise(for Email/Username Signup/Login), 
    -  Omniauth-facebook(做 Facebook 登录)  

Reference: Code, Readme, and [This Github Issue comment](https://github.com/sharetribe/sharetribe/issues/2525#issuecomment-246609666)

<br/>
## Model  

- Model for store user info is `person` (Table name is `people`) (app/models/person.rb)  
  not using any model name(`user` or `account`)


## Controller



<br/>
### Sidenote
Sharetribe's old name is "Kassi",  
That's why you saw `Kassi::Application.routes.draw do` in 'config/routes.rb' file.    
Reference: https://github.com/sizzlelab/kassi     


<br/>
### About 1c7 (the guy who wrote this)   

I don't work for Sharetribe, I have a projet(not my idea) that are base on Sharetribe     
So I have to learn about how Sharetribe work, How to customize it.      
I am Ruby on Rails developer for 8 month now, That help.  





