# Development
* Tech aspects of the system
  * The tech aspect of the system is being able to login/logout and upload a video and play that video in the uploader.
* What kind of technologies are needed to replicate and how
  * The kind of technologies that are needed to replicate the project are a Windows 10 computer and Visual Studio 2019
  * These are the steps of how to replicate it:
    *   Step 1: Download and install Visual Studio 2019 with the packages shown here
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

* Required IDEs, frameworks, etc
  * Visual Studio 2019 (Packages will be installed with Visual Studio)
    * Xamarin 
    * Xamarin.forms
    * .NET
    * Azure
  * C#
* Explaining folder structure in the code repositories and what they mean
  * The structure of the code is listed by the platforms. The project is a Xamarin/Xamarin.forms project.  
  <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Platforms.png" width="400">
  
  * Then those 4 categories are separated further. Let's look at ZooomNative.UWP for example. 
  <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/UWP.png" width="400">
  
* Explaining important files, such as config files
  * Important files are similar throughout the project. This image shows these important files:
  <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Native.png" width="400">
  
  * To run tests, run ZooomUnitTests. If this does not work uncolapse ZooomUnitTests and right click serives and run tests. 

* Special section on how to test and how to interpret the result
  * Sign in screen
    * Users can sign in with Zooom credentials and the application will authenticate that you are using the right credentials. Also if the user does not have a Zooom account, they can register at the Zooom website. Another thing is, if the user forgets their password, they can change it via the link (Forgot Password) to Zooom’s website. 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/SignIn.png" width="400">
    
  * Upload
    * If the user presses the add file buttton, it will bring up a file explorer and allow the user to pick a mp4 file to add to the application.
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Upload.png" width="400">
    
  * Play Video
    * On this page, the user will be able to see what video he uploaded and be able to play that video. Also, on this screen it shows the title of what your video file is called. Another thing is, you can add details about the video. The information that you can add is, the home team, the away team, the game number, the sport, the level (minor, pro, grade school), the location of the game, and the description of the game.
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/LogOut.png" width="400">
    
    * 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/EditInfo.png" width="400">
    
    * 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/EditDesc.png" width="400">
    
    * After editing the video details, you can now upload the video to Zooom's main website. You can upload multiple videos to the website. 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/VideoUpload.png" width="400">
    
    
    * Once you hit upload go to [Zooom's webstite](https://portal.zooomapp.com/Account/Login) to login and check that the video has been uploaded. You will see a progress bar in Zooom if the video has not fully uploaded by the time you check to see if the video has uploaded. 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Zooom2.png" width="400">
    
    * 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Zooom1.png" width="400">
    
  * Log out
    * User can press the log out button and log out of Zooom account. This will delete work that was done. This is the case for this iteration. This problem is going to be solved in the future. 
     <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/LogOut.png" width="400">

