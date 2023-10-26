# **Twitch StreamElements Cheat Sheet**
Basics in Twitch Chat
[AnyUser]: **/me** `type '/me' before message to recolor text to same sender user's color`
[AnyUser]: **/w** `type /w @AnyChatter before message to whisper AnyChatter`
## How to !Command `!command == !cmd`
## 1. **Custom:**
**+ !command:**
**add//edit//show//remove//alias//options//**
```assembly
!cmd add Hello Hello World!                !Hello will send to chatbox 'Hello World!'
!cmd edit Hello Hello ${random.chatter}!   Changes 'Hello World' to 'Hello @[RandomUser]!'
!cmd show Hello                            Will show command line to chatbox 'Hello ${random.chatter}'
!cmd remove Hello                          Will remove existing '!Hello' command
```
**+ Alias:**
**-add//-remove**
```assembly
!cmd alias add Hello Hi Hiho Ahoy   Will add 'Hi', 'Hiho', 'Ahoy' as command alias
!cmd alias remove Hello Hiho Ahoy   Will remove 'Hiho', 'Ahoy' as command alias
!cmd alias Hello                    Will show 'Hi' as command alias
```
**+ Options**
**-disable//-enable//-cd//-usercd//-cost//-level[^1] //-type**
```assembly
!cmd options Hello -disable       Will disable 'Hello' command
!cmd options Hello -enable        Will enable 'Hello' command
!cmd options Hello -cd 600        Will set a global cooldown of 10 minutes to 'Hello' command
!cmd options Hello -usercd 60     Will set individual user cooldown of 1 minute to 'Hello' command
!cmd options Hello -cost 100      Will set cost of 100 'loyalty points' for 'Hello' command
!cmd options Hello -level 100     Will allow level 100 or higher to use 'Hello' command
!cmd options Hello -type reply    Will config to send to user in chatbox
!cmd options Hello -type say      Will config to send in chatbox
!cmd options Hello -type whisper  Will config to send in whisper
```
## 2. **Variables [~$]:**
### **+ Random:**
**${random.chatter}//${random.1-20}//${random.pick 'rock''paper''scissor'}//${random.emote}**
  - ${random.chatter}
```assembly
!cmd add !Hello Greetings! How are you? ${random.chatter}
[You]: !Hello 
[Bot]: Greetings! How are you? [@RandomUser]
```
  - ${random.1-20}
```assembly
!cmd add !dice ${sender} rolled a d20 and got ${random.1-20}!
[You]: !dice
[Bot]: [@You] rolled a d20 and got [19]!
```
  - ${random.pick'rock''paper''scissor'}
```assembly
!cmd add !rps ${sender} choose ${random.pick 'rock''paper''scissor'}!
[You]: !rps
[Bot]: [@You] choose [paper]!
```
  - ${random.emote}
```assembly
!cmd add !reactme ${sender} ${random.emote} ${random.emote} ${random.emote}!
[You]: !reactme
[Bot]: [@You] [NotLikeThis] [LUL] [Kappa]
```
### **+ User:**
**${user}//${user.points}//${user.level}//${user.lastactive}//${user.time_online}** 
  - ${user}//${user.name}
  - ${user.points}//${user.points_rank}//${user.points_alltime_rank}
  - ${user.level}
  - ${user.lastactive}//${user.lastseen}//${user.lastmessage}
  - ${user.time_online}//${user.time_offline}//${user.time_online_rank}//${user.time_offline_rank}
```assembly
!cmd add !
[You]: !
[Bot]: 
```
### **+ Sender:**
**${sender}//${sender.points}//${sender.level}//${sender.lastactive}//${sender.time_online}** 
- Works like `${User} Variable` but return only about sender.

> [!note]
> Always use time converted to **seconds**.

> [!important]
> Some _!command_ ***Custom*** and ***Options*** may require _user level_ to access and edit.

> [!warning]
> This Sheet is to remember me how commands work! If you learnt something, GOOD! 👍
> <!-- Do you like it and want support me? Sorry, only have [ttv/KazKazu](www.twitch.tv/KazKazu) -->

[^1]: **User Level:**
[100 = viewer] //
[250 = subscriber] auto level to 250 //
[300 = regular] //
[500 = moderator] assigned to Twitch Creator Dashboard auto level to 500 //
[1000 = super moderator] StreamElements ChatBot Feature //
[1500 = broadcaster] assigned to channel owner auto level to 1500
