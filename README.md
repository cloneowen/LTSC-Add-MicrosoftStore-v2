# LTSC-Add-MicrosoftStore-v2
# Add Store to Windows 10 Enterprise LTSC  
For Windows 10 Enterprise LTSC 2019/2021   
## To install, run Add-Store.cmd as Administrator   
If the store still will not function, reboot. If still not working, open the command prompt as the administrator and run the following command, then reboot once more.  
```PowerShell -ExecutionPolicy Unrestricted -Command "& {$manifest = (Get-AppxPackage Microsoft.WindowsStore).InstallLocation + '\AppxManifest.xml' ; Add-AppxPackage -DisableDevelopmentMode -Register $manifest}"```    
## Addition troubleshooting    
>Right click start  
Select Run  
Type in: WSReset.exe  
This will clear the cache if needed.  
  
# 为Windows 10 Enterprise LTSC增加应用商店  
适用于Windows 10 Enterprise LTSC 2019/2021    
## 要开始安装, 请打包下载后用右键管理员运行 Add-Store.cmd      
如果装完之后商店仍然打不开，请先重启试试。如果仍然不行，请以管理员身份打开命令提示符并运行以下命令之后，然后再重启试试。  
```PowerShell -ExecutionPolicy Unrestricted -Command "& {$manifest = (Get-AppxPackage Microsoft.WindowsStore).InstallLocation + '\AppxManifest.xml' ; Add-AppxPackage -DisableDevelopmentMode -Register $manifest}"```    
## 商店修复    
Win+R打开运行，输入WSReset.exe回车。    
该命令会清空并重置Windows Store商店的所有缓存。    

# 為Windows 10 Enterprise LTSC增加應用程式商店
適用於Windows 10 Enterprise LTSC 2019/2021
## 要開始安裝, 請打包下載後用右鍵管理員執行 Add-Store.cmd
如果裝完之後商店仍然打不開，請先重啟試試。 如果仍然不行，請以管理員身份開啟命令提示字元並執行以下命令之後，然後再重新啟動試用。
```PowerShell -ExecutionPolicy Unrestricted -Command "& {$manifest = (Get-AppxPackage Microsoft.WindowsStore).InstallLocation + '\AppxManifest.xml' ; Add-AppxPackage -DisableDevelopmentMode -Register $manifest}"````manifest}"````manifest}"```man
## 商店修復
Win+R開啟執行，輸入WSReset.exe回車。
此指令會清空並重置Windows Store商店的所有快取。
