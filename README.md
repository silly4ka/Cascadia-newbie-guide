# Cascadia new validator (compact) guide
![266290813-ad3e3dfe-b3dd-46a2-a49f-49a2409d603b](https://github.com/silly4ka/Cascadia-newbie-guide/assets/100471481/760f2c19-d61a-44a8-ba04-463ebe8eec88)
# Chapter 1 "Second steps"   
  
Ok, you rented hosting, installed a node on it and created a validator, now its sign blocks, right?  
To get started, you'll find useful links to community chats  like this (they will always help you there :3 )
 * [Discord](https://discord.gg/cascadia)  
^ A lot of news here 
 * [Docs](https://cascadia.gitbook.io/gitbook/)  
^ A lot of helpful info 
 * [Telegram](https://t.me/CascadiaFoundation)  
^ A lot of cute contributors 
 * [Telegram:Validators](https://t.me/CascadiaValidators)  
^ A lot of helpful validators     

Now you need to visit next platforms 
* [Zealy](https://zealy.io/c/cascadia) - Confirm some quests here
* [Coordinape](https://app.coordinape.com/join/0532e404-c13d-4b4a-92d3-29732b3738b0) - Leave reports about contributions here & encourage contributions of others with GIVE (it's important)  
^ [How to use Coordinape Guide]( https://medium.com/@CascadiaFoundation/cascadias-coordinape-handbook-63696877c898)

# Chapter 2 "Update will be at 7am, how to survive??"
Calm down it's just an update  
This is ussualy an update to the binary file   
Sounds hard? it's not, it's just a few steps
  
Open home directory
```
cd 
```
Download new binary before update height (replace v0.x.x with new version)
```
 wget https://github.com/CascadiaFoundation/cascadia/releases/download/v0.x.x/cascadiad
```
Make this file executable
```
chmod +x cascadiad
```
Replace the old file
```
mv cascadiad $HOME/go/bin/cascadiad
# or you can use
mv cascadiad ($which cascadiad)
```
Restart cascadiad
```
sudo systemctl restart cascadiad
#or
sudo systemctl restart cascadiad.service
```
Check version & status!
```
cascadiad version
cascadiad status | jq
```
Also you can check journal
```
sudo journalctl -u cascadiad -f -o cat
```
*Also check discord for additional instructions!  

*Is your console full of errors & node doesn't work?  
 ^ check [Discord](https://discord.gg/cascadia) & [Telegram:Validators group](https://t.me/CascadiaValidators) - you might have missed something - smart guys will tell you

Will update happen when you are busy and you want to update an advance??  
Don't do this, you'll have to roll back to previos version, it's better to be a ittle late, but in general you need to update on time

# Chapter 3 "My node stop sign blocks!! This is the end of the universe???"

Calm down again, check your voting power - if that less than in the top 100 Validators - ask for delegation   
Voting power is ok? - Check your version & actual, also chek journal  
```
cascadiad version
sudo journalctl -u cascadiad -f -o cat
```
If you can't identify problem - ask it in [Telegram:Validators](https://t.me/CascadiaValidators)
If you don't recieve a response for a long time, try basics things - update peers, seeds, address book, install a snapshot  
(helps beginners 90% of the time)  
You can use offical guide from [offical gitbook](https://cascadia.gitbook.io/gitbook/) or [community guides](https://cascadia.gitbook.io/gitbook/directory/guide)  

# Chapter 4 "I'm tired of copy-pasting, I want to grow!"
Good thougs friend!  
A good validator must solve problems both with and without the community  

* If it your first node & GNU/Linux exp.  
You need to learn basic commands like  
```
cd
ls
mv
cp
nano
apt-get
wget
```
When you copy-paste again & see unfamiliar command, don't be lazy, Google it!

* Now you can move around the system independetly! (achievement unlocked)
Explore your system! open varios configs(with nano) Learn new terms and discover new opportunities!  

* Also explore all the possibilities of cascadiad command  
```
cascadiad tx  
cascadiad status  
cascadiad keys  
etc  
```

All this will help you to solve your problems independently! - It's yours Second Steps!  

# Chapter 5 "My node working perfectly! What else i can do?"

* Congrats! lvl 3 reached!  
Now you can   
Help other new validators  
Popularize the project  
Make guides (like how i did it)  
In general - to contribute  

(don't forget about reports on [Coordinape](https://app.coordinape.com/join/0532e404-c13d-4b4a-92d3-29732b3738b0) & encourage contributions of others with GIVE, bye :3 )
