### Original repo: https://github.com/fuibax/fuibax.github.io

### I've converted these assets to be usable in the game ([game_files.zip](https://github.com/mmarkus13/fuibax.github.io/raw/main/game_files.zip)).<br/>To use them they need to be copied into the HotA.lod file via [mmarchive.exe](https://github.com/GrayFace/Misc/releases/download/MMArchive-1.3.1/MMArchive.rar) tool.



#### There are additional assets which are _not enhancements of the originals_ but rather [alternative portraits to heroes](https://github.com/mmarkus13/fuibax.github.io/raw/main/alternative_hero%20portraits.rar).<br/>Most of these are already either `.pcx` or `.bmp` format so they can be imported as they are.
<br/>
If you'd like to add a fully customized portraits of your own, you should follow these steps:

1. find or create pictures that you like and save them
   then you have to create two different files for each portrait:
    - small one 48x32 pixels name h***s.pcx
    - big one 58x64 name h***.pcx
<br/>(the *** is the hero number. you can take lookup these codes here: [https://heroes.thelazy.net/index.php/Hero_portraits](https://heroes.thelazy.net/index.php/Hero_portraits)
<br/>([PowerToys tool](https://github.com/microsoft/PowerToys/releases/download/v0.77.0/PowerToysUserSetup-0.77.0-x64.exe) is quite handy to have for both `mass-resizing images` and `mass renaming` if needed)
    - put both files in ~\Heroes3\Data folder (if you are only experimenting temporarly; or use the mmarchive to put them into lod file as described above)

  - If you need to convert the images from different format (jpeg/jpg/png... to bmp), then put all your images into one folder and run the following bash command:
  `for f in *.png; do convert "$f" "${f%png}"bmp; done`
2. The bmp files need to be run trough [H3DefTool](https://sourceforge.net/projects/grayface/files/H3DefTool/v3.4.2/H3DefTool.rar/download) first to appear properly in the game.
    - Open the tool and `Select "$47 Interface"` from the "Type" drop down menu in the top centre of the window
    - Go to the `"Frames"` tab in the window and navigate to your images (small and large portraits)
    - Go back to the `"General"` tab and check the `Bitmaps box`, then press `ctrl+A` & `Enter`
     <br/>(also make sure to turn off transparency as it may negatively affect the portraits; additionally the portraits use 256-color bitmaps and the first color will always be treated as a transparency layer)
    - create an export folder; if you make it the same as the import folder, it will OVERWRITE your images! So be careful!
    - click the little icon next to the "..." at the end of the "Bitmaps" area that says `"Prepare Pictures By One"`
3. Import your new portraits as mentioned above


### Meme heroes:
![meme heroes](https://github.com/mmarkus13/fuibax.github.io/blob/main/meme%20heroes.png)
<!--
no comment
-->
