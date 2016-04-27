#How to Use Movie Textures to Play 2D Animations

![Header]
(http://alistapart.com/d/_made/d/ALA_428_Safer-Web-Animation_960_251_81.jpg)
######By Morgan Maslow

##Introduction
For our project we wanted to have 2D animations play during our Start and Restart screen. We thought that simply importing them would do the trick. This proved to not be the case since it was not a keyframed animation, but a mp4 I had made from Photoshop. For those of who want moving animations in your unity games, this is how. 

##Step One: Make the Animation
Draw an animation in software such as Photoshop or make a Render a 3D animation using After Effects. The animation MUST be a .mov file since the script used in this tutorial does NOT support other files. Photoshop renders animations out as .mp4's but you can use any pnline sources to change the file. Import .mov file into Assets Folder.

Here is a helpful conversion website: http://video.online-convert.com/convert-to-mov

##Step Two: Make a Plane 
![Plane]
(http://i.imgur.com/lgFp7XZ.png)
Create a plane in your scene. Rotate it to face the camera and adjust to make sure your plane is properly lit. If the plane isn't lit properly the animation WILL NOT show up.

##Step Three: Create Script
Create a C# file. Type the below script into the script editor:

![Script]
(http://i.imgur.com/pzvH7IM.png)

Make sure the name of the script and class match or the script will not work. 

##Step Four: Attach to Plane and Add .Mov File in Appropriate Spots 
Attach the script to the plane. Go to the inspector and add the .mov file to the Mov Texture attribute.
![Mov Texture]
(http://i.imgur.com/nLlSBMp.png)
