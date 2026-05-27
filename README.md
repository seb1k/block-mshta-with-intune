

Validate the Microsoft Secure Score recommendation:

> **Block outbound network connections from Microsoft HTML Application Host (`mshta.exe`)**


## Go to Intune > Endpoint security \| Firewall

https://intune.microsoft.com/?ref=AdminCenter#view/Microsoft_Intune_Workflows/SecurityManagementMenu/~/firewall

- **Create Policy**
<img width="141" height="101" alt="image" src="https://github.com/user-attachments/assets/0890f334-4852-42c1-8017-246e9d9654bc" />

- Platform : **Windows**
- Profile : **Windows Firewall Rules**

<img width="237" height="466" alt="image" src="https://github.com/user-attachments/assets/40dbe3f9-827d-4b9e-a785-204e3779aaa8" />

#### Basics
- Name : Block mshta.exe
- Description : Block outbound network connections from Microsoft HTML Application Host (mshta.exe)

#### Configuration Settings
- Add 2 rules :
- Block C:\Windows\SysWOW64\mshta.exe
- Block C:\Windows\System32\mshta.exe
- Set the action to **Block** for both rules.
<img width="987" height="200" alt="image" src="https://github.com/user-attachments/assets/6426149f-164d-4d74-b21f-3535bd6b15c8" />


**Rule 1 Click Edit instance :**
- Enable : **Enabled**
- Interfaces types : **All**
- File Path : Click **configure** -> **C:\Windows\SysWOW64\mshta.exe**
<img width="897" height="155" alt="image" src="https://github.com/user-attachments/assets/4c9f5186-365d-48b5-9c52-f0070b3e3fd1" />
<br/>
<img width="80" height="32" alt="image" src="https://github.com/user-attachments/assets/36ccdacc-008a-4d3b-89e5-2722200fd479" />


**Rule 2 Click Edit instance :**
- Enable : **Enabled**
- Interfaces types : **All**
- File Path : Click **configure** -> **C:\Windows\System32\mshta.exe**
<img width="906" height="157" alt="image" src="https://github.com/user-attachments/assets/7311b907-8ed0-4a01-a0e1-d952d286cc0a" />
<br/>
<img width="80" height="32" alt="image" src="https://github.com/user-attachments/assets/36ccdacc-008a-4d3b-89e5-2722200fd479" />


#### Scope Tags
Nothing
#### Assignements
- **All devices**
<img width="304" height="147" alt="image" src="https://github.com/user-attachments/assets/dc844e9c-23aa-4c33-bbdf-22017320966c" />


#### Review + create
<img width="88" height="37" alt="image" src="https://github.com/user-attachments/assets/e16819f6-d4e7-4958-b5c5-30de618b00eb" />



