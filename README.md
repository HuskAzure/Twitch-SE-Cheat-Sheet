# **Twitch StreamElements Cheat Sheet**
### Basics in Twitch Chat
[UserWithBlueColor]: **/me** _<-- Before message recolor text to user **blue** color._
### How to !Command
`!command == !cmd`
- Custom: add//edit//show//remove//options//alias
  - !cmd add Hello Hello World!
    `!Hello will send in chat 'Hello World!'`
  - !cmd edit Hello Hello ${${random.chatter}}! `Changes 'Hello World' to 'Hello @[RandomUser]'`
  - !cmd show Hello `Will show command line in chat "Hello ${sender}"`
- Options _-Flag_: -enable//-disable//-cd//-usercd//-cost//-type//-level
  - -enable
  - -disable
- Variables [~$]:
  -Random: ${random.chatter}/${random.0-100}/${random.pick'rock''paper''scissor'}

> [!note]
> Always use time converted to **seconds**.

> [!important]
> Some _!command_ ***Custom*** and ***Options*** will require _user level_ to access.
- User Level: [100 = viewer], [250 = subscriber], [300 = regular], [500 = moderator], [1000 = super moderator], [1500 = broadcaster]
  - subscriber auto level to 250
  - moderator assigned to Twitch Creator Dashboard auto level to 500
  - super moderator
  - broadcaster assigned to channel owner auto level to 1500
> [!warning]
> This Sheet is to remember me! If you learnt something, GOOD! 👍
> 
