# chocolatey-Installation </br>
Open PowerShell as Admin and type: (this will makesure all resources to be install from Choco get **Audit signed**) </br>
```Set-ExecutionPolicy AllSigned```

Install Chocolate
```java
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```
No need to restart the console</br>

Example to install Apps:</br>
```Java
choco install git -y
```
Example to Uninstall</br>
```Java
choco uninstall git -y --remove-dependencies
```

To get more info utilizing the tool</br>
```choco -h```
