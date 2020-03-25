# Movies for the SDD lessons

Movies for SDD lessons (Science des données biologiques, see https://biodatascience-course.sciviews.org) are made using Movavi Video Editor 15 (MVE). On the contrary to iMovie, MVE does not creates a big file with all the media in it, but points to the original files and keeps only a small project file. That project file can be easily versioned on Github, as in the present repository.

Now movies media and outputs that are too voluminous to be stored on Github should be stored elsewhere. We use a pCloud drive of 2Tb dedicated to SDD to store that voluminous material (rushes, voices, screencasts, ...) and leave only the Movavi Video Editor projects versioned on Github. In order to use the `sdd_movies_data` folder in a reproductible way from machine to machine, one has to create a *symbolic link* in the same root folder where `sdd_movies` is cloned on your disk.


## MacOS procedure

On the Mac, open a terminal and go to the base folder where you placed the clone of the `sdd_movies` repository, then type:

```
ln -s ~/pCloud\ Drive/sdd_movies_data sdd_movies_data
# Check
ls -l # The sdd_movies_data folder should point to pCloud drive
```

Now, your MVE projects will use the media that are stored into `sdd_movies_data` on the pCloud drive! If MVE does not finds them when you open a project, just select the `sdd_movies_data` directory in your p-Cloud drive, and it should correct all file paths automatically.

## Windows procedure

To acces your media more easily, you can create a shortcut to `sdd_movies_data` on your p-Cloud drive, and place that shortcut on the same parent directory as the cloned `sdd_movies_data` repository.

If MVE does not finds the media when you open a project, just select the `sdd_movies_data` folder on your p-Cloud drive and MVE should correct and find them automatically.

