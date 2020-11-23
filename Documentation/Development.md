# Development
* Tech aspects of the system
  * The tech aspect of the system is being able to login/logout and upload a video and play that video in the uploader.
* What kind of technologies are needed to replicate and how
  * The kind of technologies that are needed to replicate the project are a Windows 10 computer and Visual Studio
  * These are the steps of how to replicate it:
    * In Progress

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

* Special section on how to test and how to interpret the result
  * Sign in screen
    * Users can sign in with Zooom credentials and the application will authenticate that you are using the right credentials. Also if the user does not have a Zooom account, they can register at the Zooom website. Another thing is, if the user forgets their password, they can change it via the link (Forgot Password) to Zooom’s website. 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/SignIn.png" width="400">
    
  * Upload
    * If the user presses the add file buttton, it will bring up a file explorer and allow the user to pick a mp4 file to add to the application. 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Upload.png" width="400">
    
  * Play Video
    * On this page, the user will be able to see what video he uploaded and be able to play that video. Also, on this screen it shows the title of what your video file is called. 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/LogOut.png" width="400">
    
  * Log out
    * User can press the log out button and log out of Zooom account. This will delete work that was done. This is the case for this iteration. This problem is going to be solved in the future. 
     <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/LogOut.png" width="400">

