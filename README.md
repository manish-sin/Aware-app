# Aware

Aware is a tool to help you monitor self-efficacy (your confidence to finish a task in target time) while working on PC.

### How does it work?
It 
  - logs the name of active window and duration of activity on it
  - produces a report of logs in a meaningful way

### Features

  - It works locally on your PC and does not require internet; Hence it is highly safe as it doesn't share data over the internet
  - The report is accessible on your browser itself
  - Reports are interactive and easy to explore, with a clean interface.
  - Configurable for "Start on PC startup"
  

### Use case

- Case 1: Every professional estimate the time he will require to finish a task, before hi start, whether the task it to finish a report or photoshop an image He/she will be able to monitor that by knowing how long did he use certain applications to achieve his task. If this is done on a regular basis he/she will be able to calibrate his self-efficacy. 
For example: If I had decided to finish writing a certain part of this software, I should ask myself should I have taken 148 mins?
Fig 1:
<img src="Screenshot/App.png" width=600 >
- Case 2: Looking into detail of each app you can further filter out your NVA and distraction, like while doing a course, you spent more time on Netflix to freshen up. For me take away was I spent a lot of time searching emails, which means I have not organized my mail well (of course screenshot does not show my mail i.e ;). I will improve on that.
Fig 2: 

<img src="Screenshot/Sub-app.png" width=600 >

- Case 3: You may think of more and let us know ;)

### Instalation
#### Install & Uninstall
1. Download the app repository
2. Aware.exe is the setup file, click to install the program
3. Allow the Administrator to install, by clicking "yes".
4. When the process is completed, below shown screen will appear. Please click "close" to complete the installation.

<img src="Screenshot/install Dialog box.png" width=300 >




#### Start Stop Instruction
1. After installation is complete, On Desktop you would find the <img src="Screenshot/bar.png" width=20 > icon double click it, when window as shown appears, it means app is up and running.
<img src="Screenshot/install window.png" width=600 >
2. To stop the service, close the window.


#### Configure on startup of laptop 
1. Go to the windows and open the task scheduler and refresh it.
2. Look for "aware" service and right click and run it
<img src="Screenshot/Task Scheduler.png" width=600 >
Note: On startup, it takes 10-20mins to start the aware automatically,  In case you wish to start the app on as soon as system starts, you will have to do it manually (read "Start & stop the app" instruction)

### Exploring Report
To open the report, make sure Aware is running  and then hit "http://localhost:5000/". 
- Summary of all applications used
<img src="Screenshot/Exploring_apps.png" width=600 >
- Detail of App choosen
<img src="Screenshot/Exploring_Subapps.png" width=600 >

Note:
- The sector in pie chart named "Ideal" is time for which System was in sleep mode
- The sector in pie chart named "Miscellaneous" is aggregate of all apps Nun for less than 5 minutes
- Anny window open for less than 5 sec are not logged


### FAQ:
1. Why is there always a black window, while I run the Aware?
Ans: So that you are aware that your information is being logged. Information is precious. We thought to start Aware as service was not a good idea as of know.
2. Why report shows is only for 3 days?
Ans: We feel making a repository of such a report will lead to procrastination. Making this report temporarily motivates one to act to take decisions.
3. Does it track other activities such as Mouse?
Ans: No it doesn't track anything else accept Name of Active Window.
4. Is data logged by Aware safe?
Ans: All logs are saved on your PC locally, it not sent over the internet. The code for Aware is available, you may check it.
5. Some of the items among Horizontal bars has value zero, what does that mean?
Ans: All the values shown are in minutes, hence Zero minutes mean that windows were open for less than a minute.
6. Why does it require admin permission?
Ans: Permission is required to set the app to start on start-up
