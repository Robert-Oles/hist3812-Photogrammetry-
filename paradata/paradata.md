# paradata
Macro Paradata: the big decisions relating to the nature of the visualisation.

    Why has the resource being created and for what audience? _(SG says: interpret this as asking you to tie your work into the big themes, issues, from this course)_

    How will the resource be put to use? Is it sustainable and accessible?
    
    This resource can be put to use for demonstrative purpose to show how an individual with small understanding of the finer details of photogrammetry can utilize a blend of commericial and opensource software to create basic 3d models from camera phone photos. As for the sustainablitity and accessiblity of this resource and its creation, it depends. While the process of creating this model relied on using SCANN3D's guided photo mode, a user could likely get similar if not better results taking the photos manually. As for the rest of the software, regard3d remains as an open source software that operates on all three of the major operating systems which means that it is easily acecssible and likely sustainable due to its open source nature. However, EXIF Pilot, the software utilized to alter the metadata of the photoset, is free for download but is impacted by the fact that in order to do "batch" meta data editing it requires a purchase of a plug-in totalling $79.99 USD. This is problematic because it limits this process to the smaller datasets which further impacts the quality of the model.

    Why have you chosen to use the approach/methods applied? _(SG says intrpret this to reflect on your actual process - what worked, what didn't, given the kinds of guidance or advice you've been able to find?)_
    
    This process as informed from a number of sources, firstly, Shawn Graham's lecture materials directed me to the SCANN3D application for the Android OS. This software worked in the sense that it helped in guiding me in taking these photos, but failed completly when trying to render any form of model that looked even remotely close. In the one model that was successfull, it produced a concaved version of the target which is available to view on this github account. However, Regard3d was fantastic as a piece of software that was relativly easy to use to create this software. It is important to note, that it failed to properly calibrate 32 of the 36 "cameras" however it still managed to create a recognizeable partial model that was significantly better than what was produced by SCANN3D
Micro Paradata: the small-scale decision-making processes underlying the construction of the visualisation.

    What are the basic steps you followed in putting together the resource?
**Step One**

Start by clearing any snow or debris from the statue that may impact the model
Ensure you can walk a full 360 around the subject
Start by opening the SCANN3D app and selecting New Model and the guided photo mode
Take a photo of the object and begin walking around the model ensuring you try and maximize the "green dots" on the subject as you move around the object taking more and more photos

**Step Two**

Upload the the photos to your computer

**Step Three**

Open EXIF Pilot

Select your photos from your photoset

Select a photo and edit its EXIF Pilot by adding a tag titled "Focal Length" and then the fraction value of your cameras focal length

Edit the Camera Model and Manufacturer so that it is detectable by Regard3d

Repeat until all photos in the photoset are complete

**Step Four** 

Open Regard3D and create a new project

Click add picture set

Drag and drop your photos into regard 3D

Look at the camera model and camera manufacturer colomns, if they are empty that than means you need to edit the sensor database (Step 5)

**Step Five** 

Create a new text file using a program such as Notepad++ 

Copy and paste: https://raw.githubusercontent.com/openMVG/CameraSensorSizeDatabase/master/sensor_database.csv into the new text file

Add the phone model, manufacture and sensor width of the camera in this format: Manufacturer;Model;Width

Save as: sensor_database.csv

**Step Six** 

Click compute matches

Select a keypoint sensitivity as ultra or 0.0001

leave all other settings to default 

Let it render

**Step Seven**

Begin Triangulation

Using these settings:[![https://gyazo.com/72fd5efb069d968b96811db62e8bf2a6](https://i.gyazo.com/72fd5efb069d968b96811db62e8bf2a6.png)](https://gyazo.com/72fd5efb069d968b96811db62e8bf2a6)

**Step Eight**

Begin Densification

Using these settings: [![https://gyazo.com/b40ab3458496974f2172519624722bb9](https://i.gyazo.com/b40ab3458496974f2172519624722bb9.png)](https://gyazo.com/b40ab3458496974f2172519624722bb9)

**Step Nine** 

Begin Surface generation

Using these settings: [![https://gyazo.com/4126ccde76ad898d1b16deeb7e8cb57a](https://i.gyazo.com/4126ccde76ad898d1b16deeb7e8cb57a.png)](https://gyazo.com/4126ccde76ad898d1b16deeb7e8cb57a)
    What supporting evidence did you rely upon?

    How have you acknowledged uncertainty in the resource? Where might alternative interpretations have been made or where are such interpretations otherwise available for viewing audiences to refer to?

References

McCurdy, L. (2010). Visualising Architecture: The Experience of Creating Virtual Reconstructions. Unpublished Master's thesis, University of York, UK.

