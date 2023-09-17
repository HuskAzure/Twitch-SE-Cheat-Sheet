# **Twitch StreamElements Cheat Sheet**
### Basics in Twitch Chat
[UserWithBlueColor]: **/me** _<-- Before message recolor text to user color._
### How to !Command
`!command == !cmd`
+ Custom: add//edit//show//remove//alias//options//
  - !cmd add Hello Hello World! `!Hello will send in chat 'Hello World!'`
  - !cmd edit Hello Hello ${${random.chatter}}! `Changes 'Hello World' to 'Hello @[RandomUser]'`
  - !cmd show Hello `Will show command line in chat "Hello ${sender}"`
  - !cmd remove Hello `Will remove existing command`
+ Alias function:
  - !cmd alias add Hello Hi Hiho Ahoy `Will add 'Hi', 'Hiho', 'Ahoy' as command alias`
  - !cmd alias Hello `Will show 'Hi', 'Hiho', 'Ahoy' as command alias`
  - !cmd alias remove Hello Hiho Ahoy `Will remove 'Hiho', 'Ahoy' as command alias`
+ Options _-Flag_: -disable//-enable//-cd//-usercd//-cost//-level[^1]//-type
  - !cmd options Hello -disable `Will disable 'Hello' command`
  - !cmd options Hello -enable `Will enable 'Hello' command`
  - !cmd options Hello -cd 600 `Will set a global cooldown of 10 minutes in 'Hello' command`
  - !cmd options Hello -usercd 60 `Will set individual user cooldown of 1 minute in 'Hello' command`
  - !cmd options Hello -cost 100 `Will set cost of 100 loyalty points for 'Hello' command`
  - !cmd options Hello -level 100 `Will allow level 100 or higher to use 'Hello' command`
  - !cmd options Hello -type 
+ Variables [~$]:
  + Random: ${random.chatter}/${random.1-20}/${random.pick'rock''paper''scissor'}
 
> [!note]
> Always use time converted to **seconds**.

> [!important]
> Some _!command_ ***Custom*** and ***Options*** will require _user level_ to access.

[^1] User Level:
```
[100 = viewer][250 = subscriber][300 = regular]
[500 = moderator][1000 = super moderator][1500 = broadcaster]
```
  - subscriber auto level to 250
  - moderator assigned to Twitch Creator Dashboard auto level to 500
  - super moderator
  - broadcaster assigned to channel owner auto level to 1500

> [!warning]
> This Sheet is to remember me how commands work! If you learnt something, GOOD! 👍
> Do you like it and want support me? Sorry, ttv/KazKazu
