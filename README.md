# Internship Report

## Google Summer of Code '22 @ OWASP

### Contributor Details

- **Name:** Digvijay Bhosale
- **College Name:** IIT (BHU) Varanasi
- **GitHub ID:** DigvijayBhosale1729
- **E-mail ID:** digvijayb1729@gmail.com
- **Organisation:** OWASP Foundation
- **Project:** SecureTea Project
- **Mentors:** adeyosemanputra & rejahrehim
- **Proposal:** Improving SecureTea firewall, IDS, adding a persistent AntiVirus, remote monitoring and better GUI
- **Proposal URL:** https://summerofcode.withgoogle.com/programs/2022/projects/SeyZbhc4

## Project details 

The OWASP SecureTea Project focuses on providing a one-stop security solution for various devices (personal computers / servers / IoT devices) with multiple notifier integrations - GMail, Whatsapp, SMS, Telegram, Discord, Twitter, Slack, AWS - and a complete security toolset including - AntiVirus, Persitent Malware Detection, Firewall, WAF, IDS(Intrusion Detection System), Server Auto Patcher, Log Management, IOT Security and Social Security.

### Proposal

OWSAP SecureTea requires a few updates to its features. These are 
- Improvements in IDS and FireWall 
- Complete Web GUI and Remote Monitoring 
- Shift Backend REST API from Flask to Django 
- Improve Web App FireWall GUI 
- Fixed bugs in Angular Frontend 
- Fix all issues and ensure Zero Bugs 

For Improvements pertaining to GUI 
- The Angular Frontend contains several bugs 
- * GUI looks very different in different Browsers 
- * Scrolling changes font and textboxes for the duration of the scroll Changes to the Angular GUI will fix these bugs and will improve User Experience 
- Implement “Hover for Details’ for critical symbols

### Summary of Work done

#### Updated All Notifiers

- Updated Telegram Notifier using BotFather
- Updated Twilio SMS and Whatsapp
- Removed Twitter Notifier because twitter no longer supports APIs

![telegram](https://user-images.githubusercontent.com/70275323/192230244-0516d709-0ed7-41f8-bf37-ffd8e574ea3e.jpg)


#### Created New Django API

- Created REST API for SecureTea Server using Django REST-FRAMEWORK
- Added 17 API Endpoints 
- Implemented login using secure cookies hashed using `SHA-256` Algorithm
- Django API Admin Page provides a central GUI to monitor and edit all users

**Filesystem**

![sec_server](https://user-images.githubusercontent.com/70275323/192229630-cae12fa5-c37c-4323-adb2-5932fa8043a6.png)

<br>

**API EndPoints**

<br>


![Screenshot from 2022-09-09 03-42-16](https://user-images.githubusercontent.com/70275323/189235173-00e933e2-420e-441f-ae55-d2d79f309bdf.png)
![Screenshot from 2022-09-09 01-40-57](https://user-images.githubusercontent.com/70275323/189228099-1c57577e-2d94-45fd-a25a-bff4d9402b88.png)
![Screenshot from 2022-09-09 01-42-25](https://user-images.githubusercontent.com/70275323/189228104-85e41f46-b612-4923-b2f9-024b84041d45.png)
![Screenshot from 2022-09-09 01-43-12](https://user-images.githubusercontent.com/70275323/189228106-5331ff8b-cdfb-4386-aec4-c670d6a2bbc8.png)
![Screenshot from 2022-09-09 01-43-56](https://user-images.githubusercontent.com/70275323/189228110-ce31d910-ccfd-4988-8063-0ad8e3bc94a2.png)
![Screenshot from 2022-09-09 01-49-07](https://user-images.githubusercontent.com/70275323/189228114-2b946349-3bb4-4502-85f2-57f1f4bd191a.png)
![Screenshot from 2022-09-09 01-49-24](https://user-images.githubusercontent.com/70275323/189228118-cf879c4e-6b1a-4407-9138-45449de89302.png)
![Screenshot from 2022-09-09 01-49-46](https://user-images.githubusercontent.com/70275323/189228122-5aac3501-8e04-47b8-8723-236d9b94c676.png)
![Screenshot from 2022-09-09 01-49-53](https://user-images.githubusercontent.com/70275323/189228127-831faac6-4d93-435a-9641-66dd75853f0f.png)
![Screenshot from 2022-09-09 01-50-13](https://user-images.githubusercontent.com/70275323/189228132-27e82882-3420-4822-99e7-56088d60086c.png)
![Screenshot from 2022-09-09 01-50-20](https://user-images.githubusercontent.com/70275323/189228137-c6911508-d38e-4760-a40c-159379168663.png)
![Screenshot from 2022-09-09 01-50-28](https://user-images.githubusercontent.com/70275323/189228140-ef68eb59-4302-4e72-8c00-99c227ad8d04.png)

#### Created New GUI using React

- New Clean, conscise and reponsive GUI
- Implemented Login using Cookies
- Easy to understand structure making it easy for future developers

**Filesystem**

![react_gui](https://user-images.githubusercontent.com/70275323/192230131-d1091270-6c50-4802-ad9b-322ab8ddee37.png)

<br>

<br>


![Screenshot 2022-09-26 132921](https://user-images.githubusercontent.com/70275323/192227686-a094f952-0fb7-49a9-9444-c04a858e205b.png)
![Screenshot 2022-09-26 132953](https://user-images.githubusercontent.com/70275323/192227700-963f83ac-fed8-465c-9f5c-bec3f47670f3.png)
![Screenshot 2022-09-26 133015](https://user-images.githubusercontent.com/70275323/192227710-02b83d4d-069c-45ed-ae76-fb9fc28e8240.png)
![Screenshot 2022-09-26 133037](https://user-images.githubusercontent.com/70275323/192227717-3441222b-9d99-4fb6-b7f2-80b962165e4c.png)
![index](https://user-images.githubusercontent.com/70275323/192227720-0a11b1b9-217c-41c9-91b4-26589e744af1.jpg)

#### Fixed existing bugs

- Existing bugs in securetea have been fixed
- GaussianNB instances upgraded from depreciated method to new method
- Fixed errors related to debug option
- Fixed filesystem bugs
- CSV file name error fixed

### Pull Requests and Commits 

| PR | Description | Lines Coded
| --- | --- | --- |
| [#367](https://github.com/OWASP/SecureTea-Project/pull/367) | Created Django API |  `+7,025 −6,829`  |
| [#368](https://github.com/OWASP/SecureTea-Project/pull/368) | Implemented Login via `SHA-256` hashed cookies | `+806 −32` |
| [#369](https://github.com/OWASP/SecureTea-Project/pull/369) | Fixed errors in Notifiers - Twitter, Telegram, Discord, Twilio | `+74 −55` |
| [#370](https://github.com/OWASP/SecureTea-Project/pull/370) | Created React Frontend | `23,181 −1,957` |
| [#372](https://github.com/OWASP/SecureTea-Project/pull/372) | Finalized React Frontend with all API calls and login | `+13,838 −29,266` |
| [#375](https://github.com/OWASP/SecureTea-Project/pull/375) | Fixing minor errors in frontend and libs | `+239 −3,630` |
| [#376](https://github.com/OWASP/SecureTea-Project/pull/372) | Fixed minor issues with the securetea libs | `+25 -24` |

Total Lines of Code committed  +45,188 -41,793

https://github.com/OWASP/SecureTea-Project/commits?author=DigvijayBhosale1729

### Acknowledgement

I would like to thank my mentors [(@adeyosemanputra)](https://github.com/adeyosemanputra) and [(@rejahrehim)](https://github.com/rejahrehim) for constantly guiding and helping me along, resolving my doubts, reviews and constructive criticism and positively cultivating my interest in Security and Open Source. Due to their efforts i was able to complete all objectives for this project. I would like to thank the OWASP Foundation for letting me contribute to this project and providing a wide base of other contributors and mentors to learn from. I would also like to thank the members of the SecureTea Telegram and OWASP Whatsapp group for helping me with this project, and my college peers who motivated and inspired me to complete this project.
