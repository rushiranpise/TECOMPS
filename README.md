<p align="center">
  <img src="https://raw.githubusercontent.com/rushiranpise/TECOMPS/main/icon.svg" width="75" height="75"/>
</p>

<h1 align="center">TE Comps</h1>

*TE Comps is a web browser extension for Google Meet to Auto join and Auto leave Lectures*

### Installation Instructions
**Google Chrome / Kiwi Browser** (Other Chromium Based Browsers Supported)
1. Download this [ZIP file](https://kutt.it/hqQeC4).
1. Unzip the file and you should have a folder named `TE Comps`.
1. In Chrome/Kiwi go to the extensions page (`chrome://extensions` or `kiwi://extensions`).
1. Enable Developer Mode.
1. In the top bar on the page, click on "Load unpacked"
1. Select the unzipped folder TE Comps.
1. The extension is now ready to use.

### Features
* Auto Join 5 mins before (or custom time)
* Auto Leave after specified time
* Custom Schedules
* Auto Update Time Table
* Set Default Google User Account to join Lecture

## Tech stack

React JS ⚛️ has been used in frontend and the backend workflow is established mainly using `chrome.storage` and `chrome.alarms` ⏰

## Description

![image](https://user-images.githubusercontent.com/37355997/126126839-4bc41b20-e6e4-4136-a3fb-eb24460c68d9.png)
![image](https://user-images.githubusercontent.com/37355997/126126964-2d0bf56c-3fe2-461d-bc42-b48a89ee7d30.png)

- To add an Schedule, add the link and set the start and end (optional) time in the `Custom` Tab
- LTCE TE Comps students can also select from the Abbr. and Subject list in the `Time Table` Tab
- The switch on the top is an on/off switch for the extension. If you turn it off, no schedules will get triggered.

![image](https://user-images.githubusercontent.com/37355997/126127042-85fa695c-6f9b-4ac9-891f-38926885fefe.png)
![image](https://user-images.githubusercontent.com/37355997/126127073-570d5377-c9ae-412c-97fb-c90e7c739ab0.png)

- The `Scheduled` tab shows a list of all the Scheduled

- The `Upcoming` tab shows you the Scheduled set for _Today_, _Tomorrow_ and _Later_
  - If you want to urgently join the meeting, just click on the course code given in the list. It will take you to the meeting!
  - If you want to silent an schedule or don't want it to execute because of some reason, click on the `tick mark` on the left to turn it off/on.
 
![image](https://user-images.githubusercontent.com/37355997/126127580-376576a0-5a2d-4451-bd9e-de7008f1fb8c.png)
![image](https://user-images.githubusercontent.com/37355997/126127263-59ef5f52-9fe4-45ef-b969-fc6dc63571d9.png)

- The most important thing for the auto join feature to work is the `Select Default User Account` and the `Auto Join` switch in the <b>Settings</b> tab.
  Similarly, the auto leave function won't work if the `Auto Leave` switch is turned off.

- If the Auto Join switch is turned off in the Settings tab, Schedule will execute and the link will get opened but it won't auto join the meeting for you.
- If the Auto Leave switch is turned off in the Settings tab, the Auto Leave feature won't work even if you had entered the end time.

- You can even customize the start time according to you. By default the start time is set to 5 min before the meeting time. What this means is that if the alarm is set for _10:00:00 am_, the link will get opened at _9:55:00 am_. One can change it to anything according to his/ her convenience.

### Based on 
https://github.com/devlup-labs/meet-scheduler
