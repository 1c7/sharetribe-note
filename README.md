# Here is some note about Sharetribe 
(I start this at Sep/10/2016)  
![image](https://cloud.githubusercontent.com/assets/1804755/18500223/29eac7f8-7a78-11e6-8310-ee605af4c528.png)

<br/>
## Table of Contents
  1. [What is Sharetribe?](#what-is-sharetribe?)
  1. [This Note base on What Version of Sharetribe? Answer: 5.11](#this-note-base-on-what-version-of-sharetribe-answer-511)
  1. [How to pay? (on Sharetribe)](#how-to-pay?-(on-sharetribe))
  1. [About Company](#about-company)
  1. [Website that base on Sharetribe](#Website-that-base-on-Sharetribe)
  1. [Tech Stack](#tech-stack)
  1. [Sidenote](#sidenote)
  1. [Code](#code)
      * Model
      * Controller
      * View

<br/>
## What is Sharetribe?
Sharetribe is this:       https://www.sharetribe.com/   
[About](https://www.sharetribe.com/about.html)  
[Team](https://www.sharetribe.com/team.html) 

Open Source Code is here: https://github.com/sharetribe/sharetribe   

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
Not a complete list, because even sharetribe offcial don't know exactly how many website base on sharetribe  
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
- React + jQuery
- "what you see is what you get" Editor [Mercury](http://jejacks0n.github.io/mercury/)  
- Deploy: Custom Script (not using Mina or Cap3)  
- Server: Heroku (BaaS)  
- Image Hosting: Amazon S3  
- Notable Gem: 
    -  devise | for Email/Username Signup/Login
    -  omniauth-facebook | Third party login: Facebook
    -  haml | easier to write HTML
    -  mysql2 | because sharetribe using mysql
    -  paperclip | image upload
    -  passenger | rails server
    -  react_on_rails | yep, react
    -  factory_girl, capybara, rspec-rails, cucumber-rails, selenium-webdriver | for test

Not really sure they are using: Spinhx (I don't know how this thing work)  


<br/>
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

### 1. Below is what I think, not 100% correct
because I don't work for Sharetribe. I am not team member.     
I am just guessing and testing and poking around, trying to understand how they work, 
some of my guess may be wrong.    

### 2. Goal of Code Section  
Help you understand the big picture of Sharetribe.  
Here is **not** gonna write all these little detail.  
the format below may change.   

<br/>
## Model (app/models/)

- User information:  model for store user info is `person` (Table name is `people`) (app/models/person.rb)  
  there are no model name `user` or `account`


<br/>
## Controller (app/controllers/)
  
  - application_controller (600 line) - a lot function
  
  - errors_controller (80 line) - for error, like 404, 500, 410 and so on 
  
  - homepage_controller - (300 line) for home page

  - i18n_controller - (10 line) only 1 function: change language and redirect, that's it

  - landing_page_controller - (300 line) landing page
  
  - design_controller - (4 line) show design compoment 



<br/>
## Database Table (db/schema.rb)

  - people | store user infomation, include: given_name, family_name, email, password, so on
  
  - communities | very import table, 85 field.
  
  - locations | lat, lng, string address
  
  - messages | I think that's how 'inbox' work

  - follower_relationships  | A follow B


<br/>
<br/>
## About 1c7 (the guy who wrote this)   

I don't work for Sharetribe, I have a projet(not my idea) that are base on Sharetribe     
So I have to learn about how Sharetribe work, How to customize it.      
I am Ruby on Rails developer for 8 month now, That help.  

(I am living in GuangZhou, China, I am 21 years old(1995))

---

File beside `readme.md` you don't have to look inside, because these are unfinished note.  
I would put link in readme once it finished, so you don't have to worry about it.  

(I am not native English speaker, if you spot any grammar error, Please point out help me improve, Thanks)




