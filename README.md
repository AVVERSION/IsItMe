![ISITME](https://github.com/user-attachments/assets/fef1b917-4ed0-4fdc-9358-dbb2ddc7854f)

**To Install IsItMe onto your Windows Device,**
 
1. Download the Zip File and extract it on your device.
2. Open the Extracted Folder and drag the IsItMe.exe file into the Startup Folder in the same directory.

IsItMe will now run whenever the Computer is turned on after shutdown or restart.

**If you wish to run it automatically whenever the computer is turned on after sleep or hibernation,**

1. Go into the folder and click on the address bar at the top of the window
![image](https://github.com/user-attachments/assets/6eb7ee00-d982-4c86-b49c-4500b19b4c51)
2. Copy the address using `Ctrl + C` or Right Click and Press Copy
3. Open PowerShell as an Administrator
![image](https://github.com/user-attachments/assets/363dfdfe-efda-4bca-a5ae-24043341d69d)
4. Type `cd ` and then press `Ctrl + V` or Right Click to Paste the Address and press `Enter`
5. Copy and paste the commands mentioned one by one below\
- `$originalPolicy = Get-ExecutionPolicy`\
- `Set-ExecutionPolicy RemoteSigned`\
PowerShell will display a message. Press `Y` and `Enter`\
- `.\runOnWake.ps1`\
Powershell should display a success message.\
- `Set-ExecutionPolicy $originalPolicy`\
PowerShell will display a message. Press `Y` and `Enter`

Now IsItMe will run even when the computer is woken up from sleep or hibernation.
