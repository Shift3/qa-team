# Project Name
This project is a WordPress website for the (Project name) for users to receive information about the organization, more information about creating and acceptance test. This sprint will focus on functionality of the site, ADA compliance, mobile-friendliness, and ensuring it looks good across evergreen browsers (Chrome, Firefox, and Safari). This Sprint, it will focus on the following pages: About, Contact Us/Form, Comments, and embedded videos.
## Project-Under-Test
https://Example.Example.com/testingexample
## Timeframe
Kickoff: 9/18/2020
Start Testing: 9/21/2020 
End Testing: 9/25/2020
## Browser and Device Requirements
Windows devices
Android devices
Chrome, Safari, Firefox
# Acceptance Test
## Options
This is the dropdown menu located in the upper left corner of the application. You can view the Login, Configuration, Manual Entry, Enable Offline Mode, and Error Logs windows through this dropdown menu.
### Login
- [ ] Email and Password are both required to login to the application
- [ ] Entering an email with the wrong credentials will bring up an error message
- [ ] User cannot be logged into the application and web application at the same time
### Manual Entry
- [ ] Entering an existing session id will bring up a user session
- [ ] Entering an existing session id while logged out will show that the appointment was not 
found followed by a prompt to please log in
- [ ] User should be able to enter any session id while in offline mode (disconnected from a network) and add images
- [ ] Once brought back online, images should upload to the intended session
### Error Logs
- [ ] Error Log displays desired amount of records
- [ ] Records display when a user logged in under the date column - [ ] Records display what user logged in under the UserID column
## Offline Mode :
- [ ] A user may continue to use most parts of the application while completely disconnected from the internet
- [ ] A user can paste an image into source folder and the image will show up on the current session while offline
- [ ] An image uploaded while offline will become a new folder in the destination folder
- [ ] A user cannot save a session while disconnected from the internet
 - [ ] A user can Close Appointment while disconnected from the internet; the appointment will not update and the user will be notified about this; the images should queue for upload and upload later
## Online Mode :
- [ ] A user can open an existing session with Manual Entry option
- [ ] Attempting to open a non existing session with Manual Entry will bring up 'Session ID is not valid!' error
- [ ] Any images added to an existing user in offline mode will be uploaded
- [ ] Any images added to a non existing user in offline mode will not be uploaded and skipped over if other images are added to existing sessions
- [ ] User can edit an existing session by selecting the Edit button
- [ ] Selecting the Save button will save the changes made in Edit mode
- [ ] Flagging an appointment allows user to create a Flagged Note
- [ ] Closing an appointment will close session
## Network Handling Tests:
SID = session id (same as appointment id)
- [ ] Start logged in, no session. Disconnect internet. Enter a valid SID. Take photos while disconnected from internet. Reconnect internet. The files should be uploaded to the server.
- [ ] Start logged out (stay logged out), no session. Disconnect internet. Enter a valid SID. Take photos while disconnected from internet. Reconnect internet. Log in. The files should be uploaded to the server.
- [ ] Start logged in, no session. Disconnect internet. Enter a valid SID. Take photos while disconnected from internet. Close the app. Reconnect internet. Open the app. The files should be uploaded to the server.
- [ ] Start logged out (stay logged out), no session. Disconnect internet. Enter a valid SID. Take photos while disconnected from internet. Close the app. Reconnect internet. Open app. Log in. The files should be uploaded to the server.
- [ ] Start logged in, no session. Disconnect internet. Enter an invalid SID. Take photos while disconnected from internet. Reconnect internet. The files should be discard gracefully.
- [ ] Start logged in, no session. Enter a valid SID. Take a LOT of photos (30). Disconnect Internet. Wait 5 minutes. Reconnect internet. The files should be uploaded to the server.
- [ ] STRESS TEST: Create 10 appointments. Start logged in, no session. Disconnect from Internet. Enter a valid SID. Take a LOT of photos (30). Repeat 9 more times with 9 different SIDs, 30 photos each. Wait 5 minutes. Reconnect internet. The files should be uploaded to the server.
- [ ] CRASH SIMULATION: Start uploading 30+ files. Using Task Manager, kill the application. Start the application. The remaining photos should upload. No files should be lost.

## Other:
- [ ] Usb Alert: In settings, click “add new device”. Plug in some usb device. Give it a name. Now when you unplug the device, the app should beep and show a warning message.
- [ ] Session Expires: Appointment should close when the time elapses.
- [ ] Camera App: Select any application on your computer (such as Paint). When you click on the Camera picture in the main screen, it will open that app.
- [ ] In new version, you can edit a session when offline. But what will this do?
## New Features:
- Magic Photos
- 5 minute countdown when a session start. Switches to “Running Over” and start
counting up.
