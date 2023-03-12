# TwitchBotTools
A fun little project to see how easy it is to bot Twitch views & followers without writing any actual code.
  
  ```diff
+ NOTICE: This is my passion project with the intent to show how easy it is to create and control Twitch viewer/follower Bots. Using this tool is not allowed under any circumstances and might lead to a BAN. I am not responsible for your use of the tool and the possible consequences.
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
- The tools are not perfect; you have to check on them occasionally.
  
### Advanntages & Disadvantages furthure explained.
- There are no captchas due to the way PW works. Power Automate scripts that I make use Microsoft Edge, not a dedicated browser; Power Automate uses the same Microsoft Edge you would use, while tools like selenium use a dedicated browser that has no built-up history & credibility, and thus it does not pass simple bot checks. However, the browser you use daily and build history on DOES pass bot checks.
- Some tools use Nord VPN to bypass limits (example: account creation limits) and to stay undetected. You have to have Nord VPN installed at the location `C:\Program Files\NordVPN\`. If you do not have Nord VPN installed at that location, see the below guide; the only difference will be that you will have to manually resolve problems caused by IP limitations (such as creating more than two accounts at a time). As I am aware, there is no way to remove these IP limitations apart from slowing down the program drastically.
- My program is a little slow for two reasons, 1. Avoid detection, and 2. As my program uses Nord VPN and not individual proxies, your computer has to disconnect and reconnect to a new VPN server every time an account creation is performed; this process takes time (about 7 seconds).
- While a tool is actively doing something (for example, navigating to a stream or creating an account), it mimics user input. This means that the script acts similarly to a macro during this time. Once the tool has finished its task (example: opening your stream on multiple accounts) and is not actively doing anything (example: watching a stream, not opening the stream), you are free to resume use of your device.
  
## Don't have Nord VPN installed?  
1. Go to C:\Program Files\  
2. Create a folder called `NordVPN`  

#### If you still get some error associated with Nord, VPN, CMD, Command Line, Terminal Emulator, or Console do the following:  
Delete all `CMD Session` actions, such as `Open CMD Session`, `Close CMD Sesion`, `Write to CMD Session`.
  
## Intial Power Automate Setup
#### If you DO NOT have fully updated windows 11, do the following
Note: If you have Windows 11 with the newest feature update installed, you can skip this.  
1. Go to the Microsoft Store  
2. Search and click on `Power Automate`  
3. Download `Power Automate` by pressing `Get`  
  
### Setup Browser Extension
Note: Everyone has to do this.  
1. Open `Power Automate`  
2. Press `New Flow`  
3. Enter what ever name you want, we will delete this flow right after we are done with setup.  
4. Press `Tools  
5. Press `Browser Extensions`  
6. Press `Microsoft Edge`  
7. Download the Browser Extension by pressing `Get` & `Add Extension`  
You are now finished with the initially setup of Power Automate. You can now close the window, which automatically deletes the flow.  
  
## Initial File Setup
1. Download the ZIP file [here](https://github.com/DrinkingJoe/TwitchBottingTools/archive/refs/heads/main.zip)  
2. Extract the ZIP file in the `Downloads` directory. ***THE TOOL HAS TO BE LOCATED IN THE DOWNLOADS DIRECTORY; OTHERWISE, IT WILL NOT WORK.***  
  
## Explanation of Files
- `General Password.txt` is a file used by all of the tools. Here you will enter the password you want your bots to use. There can not be any spaces, the password has to be below 25 characters, and cannot be on multiple lines.
- `twitch usernames.txt` is a file meant for account creation. Here you will enter the usernames you want your bots to use. Every username will be used only once, and if the written username is taken, the bot will use a modified username. Every username has to be on a different line. The usernames cannot have less than 4 characters and more than 25.
- `target twitch streamer.txt` is a file meant for botting followers. Here, you will enter the links of channels whose followers you want to bot. Each channel has to be on a separate line.
- `target twitch stream.txt` is a file meant for vod and stream view botting. In here, you will enter either the link to the vod (example twitch.tv/video/1568746) or the link to the stream (the new twitch link system makes streams to be located at the same URL as the streamers' accounts, example twitch.tv/nickmercs). Each link has to be on a separate line.
- `cheked twitch usernames.txt` is a file created by the `Twitch Check Accounts` tool. It is a list of accounts that have been created and verified. ***DO NOT TOUCH THIS FILE.***
- `created twitch usernames.txt` is a file created by the `Twitch Generate Accounts` tool. It is a list of accounts that have been created but not verified. ***DO NOT TOUCH THIS FILE.***
- `Modules` folder is the folder containing all of the tools.
  
## Tool Setup
- Navigate to the `modules` folder inside the `twitch botting` folder.
Here you can see all of the tools stored inside .txt files. 
#### To set up one of the tools, do the following
1. Open the .txt file of the tool you want to use; in my case, that would be the `Twitch Generate Accounts` tool.
2. Right-click and press `Select All`. Once all of the text is selected, do `ctrl+c` to copy the text.
3. Open the `Power Automate` app, and create a flow with a name relevant to the tool; in my case, I will name my flow `Twitch Generate Accounts Tool`.
4. Do `ctrl+v` to paste the text.
5. Save the flow.
Assuming that you already went through the files (as explained above) and entered the correct information, you can now start using the tool as described below.
#### To use the tool you already setup, do the following
1. Open the `Power Automate` app and find the tool you want to use.
2. Press the Play button
