PirateBox Landing Website Design
=========

Website deigns for the 0.5 (lighttpd) version of PirateBox, based on Nargren's awesome Design 2.0 (https://github.com/Nargren/PirateBox)

Still missing better mobile support, which is on its way!

Design 3.0 supports station_cnt, which is an optional modification for your PirateBox which enables you to see how many clients are connected.
To add it, please see:

http://piratebox.aod-rpg.de/dokuwiki/doku.php?id=modification_list#show_connected_clients


###---How to install---###

- Download the source code as zip or tar.gz and plug your USB stick into your computer.
- Unzip/unpack and place the contents of Design3.0 into

```
PirateBox\Shared\src\
```

- Plug the USB stick into the PirateBox and power it up.
- SSH into your PirateBox and run the following commands:

```
cd /opt/piratebox/www/
cp index.html Shared/src/old_index.html
cp Shared/src/index.html index.html
cp Shared/src/main.css main.css
cp Shared/src/pbox_small.png pbox_small.png
cp Shared/src/jquery.min.js jquery.min.js
cp Shared/src/favicon.ico favicon.ico
cp Shared/src/Flat-UI-Icons.woff Flat-UI-Icons.woff
cp Shared/src/lato.woff lato.woff
cp Shared/src/lato_700.woff lato_700.woff
cp Shared/src/lato_900.woff lato_900.woff
cp Shared/src/sk8board.jpg sk8board.jpg

```

If you have a www_alt folder, you can just place them there instead.

###---Customize---###
- Specially in Nagren's 2.0 design you can pretty much change any text in the html documents (even the image) as the layout is organized by the css file and it will not (should not) change. If you do not need for example the mobile page, feel free to remove it or do any other alterations to your copy.
- (OPTIONAL)If you already have your own forum, simply copy it over to your /piratebox/www folder and name it forum.html and complete the link to it in index.html

By default the share folder is "/Shared", if you have anything else than this please change index.html accordingly.

###---How to delete---###

```
cd /opt/piratebox/www/
cp Shared/src/old_index.html index.html
rm main.css
rm pbox_small.png
rm jquery.min.js
rm favicon.ico
rm Flat-UI-Icons.woff
rm lato.woff
rm lato_700.woff
rm lato_900.woff
rm sk8board.jpg

```

You can plug your USB stick into your computer and delete all the other files you don't need.
(A copy of the files from Design2.0 will be placed on your USB stick, under PirateBox/Shared/src/ )


###---Credits---###
Nargren for creating Design2.0.

Matthias Strubel for developing the PirateBox.

David Darts for having the awesome idea.
