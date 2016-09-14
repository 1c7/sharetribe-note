# Here is some note about Sharetribe 
(I start this at Sep/10/2016)  

<br/>
## Table of Contents
  1. [What is Sharetribe?](#What-is-Sharetribe?)
  1. [This Note base on What Version of Sharetribe? Answer: 5.11](#This Note base on What Version of Sharetribe? Answer: 5.11)
  1. [How to pay? (on Sharetribe)](#How-to-pay?-(on-Sharetribe))
  1. [About Company](#About-Company)
  1. [Website that base on Sharetribe](#Website-that-base-on-Sharetribe)
  1. [Tech Stack](#Tech-Stack)
  1. [Sidenote](#sidenote)
  1. [Code](#Code)
      2. Model
      3. Controller
      4. View

<br/>
## What is Sharetribe?
Sharetribe is this: https://www.sharetribe.com/   
Open Source Code is here： https://github.com/sharetribe/sharetribe   

[About](https://www.sharetribe.com/about.html)  
[Team](https://www.sharetribe.com/team.html)  
A Open Source Marketplace, under MIT license.   
(MIT license mean you can modify code, sell these code. only thing you have to do is keep licence file.)   


<br/>
## This Note base on What Version of Sharetribe? Answer: 5.11
All these note down below are base on 5.11  
if you find any inconsistent between Sharetribe Code and This note, Code is always right.


<br/>
## How to pay? (on Sharetribe)
Paypal    


<br/>
## About Company
Company locate at [Helsinki, Finland](https://www.google.com/maps/place/Helsinki,+Finland/@58.7019284,16.6558103,4.79z/data=!4m5!3m4!1s0x46920bc796210691:0xcd4ebd843be2f763!8m2!3d60.1698557!4d24.938379)   
People there speak Finnish 


<br/>
## Website that base on Sharetribe    
http://www.studiotime.io/  - rent music studios    
https://www.haatori.fi/ - pre-owned wedding dresses    
https://www.thequiver.com/ - rent surf board     
https://www.drivevinty.com/ - rent old car     
https://www.cyclelifehq.com/ - Bike & Bike tours    
https://www.foodforage.com.au/ - Food     
http://kamerakit.se/ - Camera     
https://app.thefoodcorridor.com/ - Food     
https://hengerdeling.no/nb?view=list - Car? this is not english..      

Reference:     
[Offcial Website: Success Story](https://www.sharetribe.com/stories.html)    
[Sharetribe Community: Marketplace Showroom](https://www.sharetribe.com/community/t/marketplace-showroom-are-you-hosting-an-open-source-sharetribe-marketplace-advertise-it-here/51/1)

<br/>
## Tech Stack (not fully comfirm by Sharetribe Team, yet.)
- Ruby 2.3.1  
- Ruby on Rails 4.2.7  
- MySQL  
- "what you see is what you get" Editor [Mercury](http://jejacks0n.github.io/mercury/)  
- Deploy: Custom Script (not using Mina or Cap3)  
- Server: Heroku (BaaS)  
- Image: Amazon S3  
- Notable Gem: 
    -  devise | for Email/Username Signup/Login
    -  omniauth-facebook | Third party login: Facebook

Reference: Code, Readme, and [This Github Issue comment](https://github.com/sharetribe/sharetribe/issues/2525#issuecomment-246609666)


<br/>
## Sidenote
Sharetribe's old name is "Kassi",  
That's why you saw 
```Ruby 
Kassi::Application.routes.draw do
``` 
in `config/routes.rb` file.    
Reference: https://github.com/sizzlelab/kassi     


<br/>
# Code  

<br/>
## Model  

- Model for store user info is `person` (Table name is `people`) (app/models/person.rb)  
  not using any model name(`user` or `account`)


## Controller



<br/>
### About 1c7 (the guy who wrote this)   

I don't work for Sharetribe, I have a projet(not my idea) that are base on Sharetribe     
So I have to learn about how Sharetribe work, How to customize it.      
I am Ruby on Rails developer for 8 month now, That help.  

Below are note I take when I am learning how sharetribe work.

File beside `readme.md` you don't have to look inside, because these are unfinished note.  
I would put link down below once it finished, so you don't have to worry about it.  

(I am not native English speaker, if you spot any grammar error, Please point out help me improve, Thanks)




