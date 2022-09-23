# TwitchBotTools
This set of tools created with Windows' Power Automate allows you to run your own Twitch Bots without any captchas for free. This includes Bot Creation, Automatic Bot Following, Botting live & vod views, and more!  
  
  ```diff
+ NOTICE: This is my pation project with the intent to show how easy it is to create and control Twitch viewer/follower Bots. Using this tool is not allowed under any circumstances and might lead to a BAN. I am not responsible for your use of the tool and the possible consequences.
```
  
## Benefits of these Tools  
- No Captchas (read more below)!
- Completely Free!
- You don't need to pay for a captcha-solving service!
- Wide Array of tools!  
- Uses NordVPN to skip limits (read more below)!
- Easy to use
  
## Disadvantages of these Tools
- A little slow (depending on your system)
- Might need a little tweaking for your system
- You can not use your system while some of the tools are running (read more below)
- You have to own a windows device
- The tools are not perfect, you have to check on them occasionally.
  
### Advanntages & Disadvantages furthure explained.
- There are no captchas due to the way PW works. Power Automate scripts that I make use Microsoft Edge, not a dedicated browser; Power Automate uses the same Microsoft Edge you would use, while tools like selenium use a dedicated browser that has no built-up history & credibility, and thus it does not pass simple bot checks. However, the browser you use daily and build history on DOES pass bot checks.
- Some tools use Nord VPN to bypass limits (example: account creation limits) and to stay undetected. You have to have Nord VPN installed at the location `C:\Program Files\NordVPN\`. If you do not have Nord VPN installed at that location, see the below guide; the only difference will be that you will have to manually resolve problems caused by IP limitations (such as creating more than two accounts at a time). As I am aware, there is no way to remove these IP limitations apart from slowing down the program drastically.
- My program is a little slow for two reasons, 1. Avoid detection, and 2. As my program uses Nord VPN and not individual proxies, your computer has to disconnect and reconnect to a new VPN server every time an account creation is performed; this process takes time (about 7 seconds).
- While a tool is actively doing something (for example, navigating to a stream or creating an account), it mimics user input. This means that the script acts similarly to a macro during this time. Once the tool has finished its task (example: opening your stream on multiple accounts) and is not actively doing anything (example: watching a stream, not opening the stream), you are free to resume use of your device.
  
## Don't have Nord VPN installed?  
1. Go to C:\Program Files\  
![image](https://user-images.githubusercontent.com/63132234/191664917-b4a177d0-bcee-40c0-9e96-acfca0dabe84.png)
2. Create a folder called `NordVPN`  
![image](https://user-images.githubusercontent.com/63132234/191664945-a7688463-3ceb-47e1-a70d-1d8a8f20c33f.png)

#### If you still get some error associated with Nord, VPN, CMD, Command Line, Terminal Emulator, or Console do the following:  
Delete all `CMD Session` actions, such as `Open CMD Session`, `Close CMD Sesion`, `Write to CMD Session`.
![image](https://user-images.githubusercontent.com/63132234/191665150-9d78274b-7dff-41c4-a60c-1f2a00cdbb2b.png)
  
## Intial Power Automate Setup
#### If you DO NOT have fully updated windows 11, do the following
Note: If you have Windows 11 with the newest feature update installed, you can skip this.  
1. Go to the Microsoft Store  
![image](https://user-images.githubusercontent.com/63132234/191665748-5dcee068-a25f-4b95-9452-19d4262d27c7.png)  
2. Search and click on `Power Automate`  
![image](https://user-images.githubusercontent.com/63132234/191665998-09e48bb4-6391-40da-a0d7-c28ccdc6e186.png)  
3. Download `Power Automate` by pressing `Get`  
![image](https://user-images.githubusercontent.com/63132234/191666227-917f98d4-5e88-4f22-9192-8ae6a4b78a81.png)  
  
### Setup Browser Extension
Note: Everyone has to do this.  
1. Open `Power Automate`  
![image](https://user-images.githubusercontent.com/63132234/191666505-b809bbe9-f1b6-48ce-9664-7800f39c3963.png)  
2. Press `New Flow`  
![image](https://user-images.githubusercontent.com/63132234/191666558-6616c1dd-79fa-4cf9-886c-a88e81930e6d.png)  
3. Enter what ever name you want, we will delete this flow right after we are done with setup.  
![image](https://user-images.githubusercontent.com/63132234/191666796-2f705005-874a-4846-9dd9-7d6c0f204108.png)  
4. Press `Tools  
![image](https://user-images.githubusercontent.com/63132234/191667665-3b2131f1-ff74-40be-bf77-b77d0a16b3d3.png)  
5. Press `Browser Extensions`  
![image](https://user-images.githubusercontent.com/63132234/191666986-f1001a2d-b19c-4dd6-b5a8-589192eaf5d1.png)  
6. Press `Microsoft Edge`  
![image](https://user-images.githubusercontent.com/63132234/191667227-1b4988b3-b5c1-42a2-a5a7-341732e3daa7.png)  
7. Download the Browser Extension by pressing `Get` & `Add Extension`  
![image](https://user-images.githubusercontent.com/63132234/191667363-0c975d3b-aa20-4615-816a-20a750da1026.png)  
![image](https://user-images.githubusercontent.com/63132234/191667435-8aadf543-ecdf-4cab-9947-fcc60a4d1680.png)  
You are now finished with the initially setup of Power Automate. You can now close the window, which automatically deletes the flow.  
  
## Initial File Setup
1. Download the ZIP file [here](https://github.com/DrinkingJoe/TwitchBottingTools/archive/refs/heads/main.zip)  
2. Extract the ZIP file in the `Downloads` directory. ***THE TOOL HAS TO BE LOCATED IN THE DOWNLOADS DIRECTORY, OTHERWISE IT WILL NOT WORK.***  
  
## Explenation of Files
- `General Password.txt` is a file used by all of the tools. In here you will enter the password you want your bots to use. There can not be any spaces, the password has to be bellow 25 characters, and cannot be on multiple lines.
- `twitch usernames.txt` is a file ment for account creation. In here you will enter the usernames you want your bots to use. Every username will be used only once and if the written username is taken, the bot will use a modified username. Every username has to be on a different line. The usernames cannot have less then 4 characters and more then 25.
- `target twitch streamer.txt` is a file ment for botting followers. In here you will enter the links of chanels who's followers you want to bot. Each chanel has to be on a seperate line.
- `target twitch stream.txt` is a file ment for vod and stream view botting. In here you will enter either the link to the vod (example twitch.tv/video/1568746) or the link to the stream (the new twitch link system makes streams to be located at the same URL as the streamers' accounts, example twitch.tv/nickmercs). Each link has to be on a seperate line.
- `cheked twitch usernames.txt` is a file created by the `Twitch Check Accounts` tool. It is a list of accounts that have been created and verified. ***DO NOT TOUCH THIS FILE.***
- `created twitch usernames.txt` is a file created by the `Twitch Generate Accounts` tool. It is a list of accounts that have been created but not verified. ***DO NOT TOUCH THIS FILE.***
- `Modules` folder is the folder containg all of the tools.
  
## Tool Setup
- Navigate to the `modules` folder inside the `twitch botting` folder.
Here you can see all of the tools stored inside .txt files. 
#### To setup one of the tools, do the following
1. Open the .txt file of the tool you want to use, in my case that would be the `Twitch Generate Accounts` tool.
2. Right click and press `Select All`. Once all of the text is selected, do `ctrl+c` to copy the text.
3. Open the `Power Automate` app, and create a flow with a name relevant tp the tool, in my case I will name my flow `Twitch Generate Accounts Tool`.
4. Do `ctrl+v` to paste the text.
5. Save the flow.
Assuming that you already went through the files (as explained above) and entered the correct information, you can now start using the tool as described bellow.
#### To use the tool you already setup, do the following
1. Open the `Power Automate` app and find the tool you want to use.
2. Press the Play button

# Before you use the botting tools, read this.
Before you start using the viewer and folower botting tools, you first need to generate bot accounts via the `Twitch Generate Accounts` tool and verify those accounts via the `Twitch Check Accounts` tool. You have to let these tools finish completely even if they seem like they are strugling. If you do not do this ***THE OTHER TOOLS WILL NOT WORK.***
