# **Twitch StreamElements Cheat Sheet**
### Basics in Twitch Chat
[AnyUser]: **/me** `type '/me' before message to recolor text to same sender user's color`
### How to !Command `!command == !cmd`
+ **Custom: add//edit//show//remove//alias//options//**
  - !cmd **add** Hello Hello World! `!Hello will send in chat 'Hello World!'`
  - !cmd **edit** Hello Hello ${random.chatter}! `Changes 'Hello World' to 'Hello @[RandomUser]!'`
  - !cmd **show** Hello `Will show command line in chat "Hello ${sender}"`
  - !cmd **remove** Hello `Will remove existing 'Hello' command`
+ **Alias function:**
  - !cmd alias **add** Hello Hi Hiho Ahoy `Will add 'Hi', 'Hiho', 'Ahoy' as command alias`
  - !cmd alias Hello `Will show 'Hi', 'Hiho', 'Ahoy' as command alias`
  - !cmd alias **remove** Hello Hiho Ahoy `Will remove 'Hiho', 'Ahoy' as command alias`
+ Options _-Flag_: -disable//-enable//-cd//-usercd//-cost//-level//-type
  - !cmd options Hello **-disable** `Will disable 'Hello' command`
  - !cmd options Hello **-enable** `Will enable 'Hello' command`
  - !cmd options Hello **-cd** 600 `Will set a global cooldown of 10 minutes in 'Hello' command`
  - !cmd options Hello **-usercd** 60 `Will set individual user cooldown of 1 minute in 'Hello' command`
  - !cmd options Hello **-cost** 100 `Will set cost of 100 'loyalty points' for 'Hello' command`
  - !cmd options Hello **-level** 100 `Will allow level 100 or higher to use 'Hello' command`
  - !cmd options Hello **-type**
+ **Variables [~$]:**
  + Random: ${random.chatter}//${random.1-20}//${random.pick'rock''paper''scissor'}
```
${random.chatter}
!cmd add !Hello Greetings! How are you? ${random.chatter}
[You]: !Hello
[Bot]: Greetings! How are you? [@RandomUser]
```
```
${random.1-20}
!cmd add !dice ${sender} rolled a d20 and got ${random.1-20}!
[You]: !dice
[Bot]: [@You] rolled a d20 and got [19]!
```
```
${random.pick'rock''paper''scissor'}
!cmd add !rps ${sender} choose ${random.pick'rock''paper''scissor'}!
[You]: !rps
[Bot]: [@You] choose [paper]!
```
> [!note]
> Always use time converted to **seconds**.
> [!important]
> Some _!command_ ***Custom*** and ***Options*** may require _user level_ to access.
- **User Level**:
```
[100 = viewer]
[250 = subscriber] auto level to 250
[300 = regular]
[500 = moderator] assigned to Twitch Creator Dashboard auto level to 500
[1000 = super moderator] StreamElements Chat Bot Feature
[1500 = broadcaster] assigned to channel owner auto level to 1500
```
> [!warning]
> This Sheet is to remember me how commands work! If you learnt something, GOOD! 👍
> <!-- Do you like it and want support me? Sorry, only have [ttv/KazKazu](www.twitch.tv/KazKazu) -->
