# Deployment 
* What kind of server is needed
  * This project is an application that runs off a users local machine and connects to a Microsoft Azure server for certain features.For user authentication, users will use their Zooom.com credentials. Primarily though, for the project to run, you just need a Windows 10 computer connected to WiFi. 
* Where to put which file/folder
  * The best place for the repository for the project is the suggested Visual Studio installation directory. For better access however, you can move the folder to the desktop for easier access.  
* How to start/stop the system
  * The way to start/stop the system is by following these steps:
    * * Step 1: Download and install Visual Studio 2019 with the packages shown here
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/packages.png" width="720">
   
    * Step 2: Go to the azure devops repository page and click the “clone” button, located next to the blue “build” button. https://dev.azure.com/thetyros/Zooom%20Website%20and%20Services/_git/Zooom%20Desktop%20Video%20Uploader 
    * Step 3: In the subsequent menu  click the dropdown menu that by default says “clone to vs code” and instead select “clone to visual studio”
    * Step 4: A window will then open in your browser, click the prompt to open visual studio.
    * Step 5: Once Visual Studio opens, make sure you are in the team explorer tab. 
    * Step 6: From there go to the bottom left hand corner and click master    
    * Step 7: After clicking on master click manage branches.
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/ManageBranches.png" width="400">
    
    * Step 8: Go to branches and click the dropdown arrow  and right click bsu-offline. 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/remotes.png" width="400">
    
    * Step 9: Then click checkout.
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Checkout.png" width="720">
    
    * Step 10: After clicking checkout, at the top of the screen you should see three dropdown boxes.
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/UWPrun.png" width="400">
    
    * Step 11: In those dropdown boxes make sure to have Debug, x64 and ZooomNative.UWP Selected.   
    * Step 12: Once those are selected hit the Green play button. 
    * Step 13: Once you have gone through the application, you can close the window that pops by clicking the red x. 

* How to troubleshoot if something goes wrong
  * First thing to do is if something is going wrong, make sure that you are on a Windows 10 device and that your current version of Windows is up to date. Another thing to check is to make sure that you have restored the NuGet packages. Also, make sure that when looking at the project in Visual Studio, that you are on the bsu-offline branch (Mentioned in steps above).
* Where to find the source of errors
  * In Visual Studio 2019, there is a tab labeled Error Lists at  the bottom of the screen (on the left hand side). This shows warnings and errors. 
* Critical/vulnerable pieces that can fail
  * The most critical/vulnerable pieces that can fail are the File Uploader, File Player, and the Login credentials. 

