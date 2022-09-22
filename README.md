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
  
## Disadvantages of these Tools
- A little slow (depending on your system)
- Might need a little tweaking for your system
- You can not use your system while some of the tools are running (read more below)
- You have to own a windows device
  
### Advanntages & Disadvantages furthure explained.
- There are no captchas due to the way PW works. Power Automate scripts that I make use Microsoft Edge, not a dedicated browser; Power Automate uses the same Microsoft Edge you would use, while tools like selenium use a dedicated browser that has no built-up history & credibility, and thus it does not pass simple bot checks. However, the browser you use daily and build history on DOES pass bot checks.
- Some tools use Nord VPN to bypass limits (example: account creation limits) and to stay undetected. You have to have Nord VPN installed at the location "C:\Program Files\NordVPN\". If you do not have Nord VPN installed at that location, see the below guide; the only difference will be that you will have to manually resolve problems caused by IP limitations (such as creating more than two accounts at a time). As I am aware, there is no way to remove these IP limitations apart from slowing down the program drastically.
- My program is a little slow for two reasons, 1. Avoid detection, and 2. As my program uses Nord VPN and not individual proxies, your computer has to disconnect and reconnect to a new VPN server every time an account creation is performed; this process takes time (about 7 seconds).
- While a tool is actively doing something (for example, navigating to a stream or creating an account), it mimics user input. This means that the script acts similarly to a macro during this time. Once the tool has finished its task (example: opening your stream on multiple accounts) and is not actively doing anything (example: watching a stream, not opening the stream), you are free to resume use of your device.
