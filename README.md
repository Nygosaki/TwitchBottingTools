# TwitchBotTools
This set of tools created with Windows' Power Automate allows you to run your own Twitch Bots without any captchas for free. This includes Bot Creation, Automatic Bot Following, Botting live & vod views, and more!  
  
  ```diff
+ NOTICE: TOOLS ARE STILL IN DEVELOPMENT
+ NOTICE: FIRST SET OF TOOLS WILL RELEASE ON 22/09/2022
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
- Some tools use Nord VPN to bypass limits (example: account creation limits) and to stay undetected. You have to have Nord VPN installed at the location "C:\Program Files\NordVPN\". If you do not have Nord VPN installed at that location, see the below guide; the only difference will be that you will have to manually resolve problems caused by IP limitations (such as creating more than two accounts at a time). As I am aware, there is no way to remove these IP limitations apart from slowing down the program drastically.
- My program is a little slow for two reasons, 1. Avoid detection, and 2. As my program uses Nord VPN and not individual proxies, your computer has to disconnect and reconnect to a new VPN server every time an account creation is performed; this process takes time (about 7 seconds).
- While a tool is actively doing something (for example, navigating to a stream or creating an account), it mimics user input. This means that the script acts similarly to a macro during this time. Once the tool has finished its task (example: opening your stream on multiple accounts) and is not actively doing anything (example: watching a stream, not opening the stream), you are free to resume use of your device.
  
## Don't have Nord VPN installed?  
1. Go to C:\Program Files\  
![image](https://user-images.githubusercontent.com/63132234/191664917-b4a177d0-bcee-40c0-9e96-acfca0dabe84.png)
2. Create a folder called `NordVPN`  
![image](https://user-images.githubusercontent.com/63132234/191664945-a7688463-3ceb-47e1-a70d-1d8a8f20c33f.png)

#### If you still get some error associated with Nord, VPN, CMD, Command Line, Terminal Emulator, or Console do the following:  
Delete all "CMD Session" actions, such as "Open CMD Session", "Close CMD Sesion", "Write to CMD Session".
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
