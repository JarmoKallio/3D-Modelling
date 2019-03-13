# 3D-model of an old hotel, a Blender project

![alt text](https://github.com/JarmoKallio/3D-Modelling/blob/master/r5.png "Final render using Blender Cycles")

This was a small hobby project of mine. I like weird and creepy looking buildings and after encountering a picture of this
nice old hotel https://thesocietyhotel.com/ decided to make a model of it. Well, its not that creepy anymore since its been renovated. The making of the thing (me modelling, not the actual construction on this ugly beauty in the times of the past) was lots of little tweaks here and there. The initial layout of things was achieved by matching a picture of the hotel to values of Blender camera. I used this excellent add-on https://github.com/mrossini-ethz/camera-calibration-pvr for camera calibration. Ater that I could move the vertices according to the lines of the building in the photograph. Okay, with this method its probably never going to be a perfect match, but I think I managed to capture the overall feeling of the building. 

At this point it's in a state of "somewhat ready and waiting use in some scene". Depending on where I'm going to use it it might still look too clean. It has some decent bumb maps now so it doesn't look like a lego house (look at the next picture and see what I mean..), but it certainly needs more dirt and more bumb and/or normal maps for the store front. We'll see what will happen! Maybe I will use it in a future project as part of a scene. I could create a night scene with creepy looking old shops for example.

![alt text](https://github.com/JarmoKallio/3D-Modelling/blob/master/r5_without_bumb.png "A lego-ish look")

The rendering engine for the time being is Blender Cycles. I used the excellent Filmic Blender rendering transform https://github.com/sobotka/filmic-blender to make the dynamic range more realistic. Some more "realism" or just better look was made possible by hdr backround. Usually I dont get that many fireflies when rendering outdoor scenes, bit this time I had to clamp down indirect ligth passes to make those white dots disappear.

The materials are not that complicated. Here is an example. Simple node setup mixing two outputs from principled shaders. Teh normal map os used for making the big (granite?!?) stones on the corners of the house, their slits. This was way easier than doing the actual modelling sincer the corners geometry can stay the same. Of course it is not that realistic when looked at closer distances.

![alt text](https://github.com/JarmoKallio/3D-Modelling/blob/master/material_nodes.png "Material nodes")

Some more pictures of the model, this time Cycles is not used.

![alt text](https://github.com/JarmoKallio/3D-Modelling/blob/master/r4.png "Wireframe look at the model")
![alt text](https://github.com/JarmoKallio/3D-Modelling/blob/master/r3.png "OpenGL render showing the model without any textures")
