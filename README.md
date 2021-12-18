# Habitat-GIF
![out](https://user-images.githubusercontent.com/62122206/146614539-a94d4d2f-47fc-475b-a3d6-ba5eeabc62fa.gif)
![out](https://user-images.githubusercontent.com/62122206/146614551-a211af81-1b78-4e72-ba21-303f2e43b7a6.gif)

### To create frames:
Edit the the original files (affinity designer: .afdesign -- or -- adobe: .psd) and export as png. 

*note: files were created with Affinity Designer (https://affinity.serif.com/en-us/) and exported as .psd for adobe compatability. adobe's layer effects are different, thus for each bud-shape you will need to adjust the inner shape's fill to be transparent and/or match the background.


### To convert pngs to gifs:

first copy the unaltered logo (00.png) as 99.png and duplicate for rest period between animation. total frames ~50. 

Install ImageMagick
```
brew install ImageMagick
```
or
```
sudo apt install imagemagick
```
cd to folder containing desired pngs, and:
```
convert -delay 1x30 *.png out.gif
```
The gif, called "out.gif" will be written into this directory.
