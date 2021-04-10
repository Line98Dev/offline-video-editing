# Development
* Tech aspects of the system
  * The tech aspect of the system is being able to login/logout and upload a video and play that video in the uploader.
* What kind of technologies are needed to replicate and how
  * The kind of technologies that are needed to replicate the project are a Windows 10 computer and Visual Studio 2019
  * These are the steps of how to replicate it:
    *   Step 1: Download and install Visual Studio 2019 with the packages shown here
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Deployment-Development-Screenshots/packages.png" width="720">
   
    * Step 2: Go to the azure devops repository page and click the “clone” button, located next to the blue “build” button. https://dev.azure.com/thetyros/Zooom%20Website%20and%20Services/_git/Zooom%20Desktop%20Video%20Uploader 
    * Step 3: In the subsequent menu  click the dropdown menu that by default says “clone to vs code” and instead select “clone to visual studio”
    * Step 4: A window will then open in your browser, click the prompt to open visual studio.
    * Step 5: Once Visual Studio opens, make sure you are in the team explorer tab. 
    * Step 6: From there go to the bottom left hand corner and click master    
    * Step 7: After clicking on master click manage branches.
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Deployment-Development-Screenshots/ManageBranches.png" width="400">
    
    * Step 8: Go to branches and click the dropdown arrow  and right click bsu-offline. 
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Deployment-Development-Screenshots/remotes.png" width="400">
    
    * Step 9: Then click checkout.
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Deployment-Development-Screenshots/Checkout.png" width="720">
    
    * Step 10: After clicking checkout, at the top of the screen you should see three dropdown boxes.
    <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/UWP-Screenshots/UWPrun.png" width="400">
    
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
  <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Deployment-Development-Screenshots/Platforms.png" width="400">
  
  * Then those 4 categories are separated further. Let's look at ZooomNative.UWP for example. 
  <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Deployment-Development-Screenshots/UWP.png" width="400">
  
* Explaining important files, such as config files
  * Important files are similar throughout the project. This image shows these important files:
  <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Deployment-Development-Screenshots/Native.png" width="400">
  
  * To run tests, run ZooomUnitTests. If this does not work uncolapse ZooomUnitTests and right click serives and run tests. 

For clipping to function, an additional step is required. FFmpeg is an additional download that is required. From the <a href="https://www.gyan.dev/ffmpeg/builds/">release section</a> on that page and download one of the "essentials" versions. Within that zip or 7z file, navigate to the folder ffmpeg-x.x.x-xxxx-xx-xx-essentials_build and then the bin folder. 

<img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Deployment-Development-Screenshots/zip.png" width="720">

Copy ffmpeg to the directory C:\Users\<username>\AppData\Local\Packages\ZoomDesktopProducer_<generated characters>\LocalState and create a folder called "ffmpeg". Now put ffmpeg.exe into that folder.

<img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/Deployment-Development-Screenshots/LocalState.png" width="720">

* Special section on how to test and how to interpret the result
  * Sign in screen
    * Users can sign in with Zooom credentials and the application will authenticate that you are using the right credentials. Also if the user does not have a Zooom account, they can register at the Zooom website. Another thing is, if the user forgets their password, they can change it via the link (Forgot Password) to Zooom’s website. 
<img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/User_Documentation_Images/LoginScreen.png" height="300">
    
  * Add Playlist
    * The user can add a playlist on this screen.
     <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/User_Documentation_Images/creating_a_playlist.png" height="300">
    
    
    * This is what it will look like after adding a new playlist.
     <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/User_Documentation_Images/default_new_playlist.png" height="300">
    
  * Edit Playlist/Upload Video to playlist
    * First you will click the 'Edit playlist' button and that will bring you to this screen. 
      <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/UWP-Screenshots/UWP-EmptyVideoView.png" height="300">
 
    * Once you have done that, you can click 'Add a video to upload' to upload a video from your device. 
      <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/User_Documentation_Images/WindowsFileExplorer.png" height="300">
    
    * Once that is done, your screen should look like this. 
    * <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/User_Documentation_Images/ListOfVideos.png" height="300">
    
    * After you have uploaded your video, you can edit the information of the playlist by clicking 'Edit the information'. Once you have done that, your screen should look like this. 
     <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/User_Documentation_Images/playlist_information.png" height="300">
    
  * Playing the Video
    * To play the video, you can play the video in the thumbnail view or you can click the 'Preview' button for a larger video player. Here is a screenshot of the video in 'Preview' mode. 
     <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/User_Documentation_Images/ClipPreview.png" height="300">
    
  * Logging off
    * If you wish to log off, go back to were all your playlists are and click the 'Log out' button.
     <img src="https://github.com/Line98Dev/offline-video-editing/blob/master/Auxiliary%20Files/User_Documentation_Images/ListOfVideos.png" height="300">
