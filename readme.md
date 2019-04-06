Vidupe 1.0
----------

Vidupe is a program that can find duplicate and similar video files.
Normal duplicate file software only finds identical files. Vidupe looks at the actual video content
regardless of different format and compression used (digital video fingerprinting).

In order for Vidupe to work, FFmpeg (http://ffmpeg.org/) must be installed:
Place ffmpeg.exe in the same folder as Vidupe.exe or in any system directory.



Features:
 - Simple, easy to use graphical user interface for comparing videos.
 - Supports all widely used video formats.
 - Multithreaded operation, makes full use of all available CPU threads.
 - Employs two powerful image comparison methods: pHash (perceptual hashing) and SSIM (structural similarity).
 - Cross-platform development: source code available for compiling on Windows/Linux/macOS.

 

Usage:
After starting Vidupe you must enter which folders to scan for video files. Folders can be added by typing them in,
dragging and dropping a folder onto the window or using the folder browser button next to the input box.
All folders must be separated by a semicolon ( ; ).

Comparison is started by pressing the "Find duplicates" button and all video files in selected folders are scanned.
A lengthy search for videos can be aborted by pressing the button again (that now reads Stop).
Note: some videos may be too broken for FFmpeg to read and will be rejected.



Settings:
The default settings have been chosen to get best results with a minimum amount of false positives.

Thumbnails:      How many image captures are taken from each video. The larger the number of thumbnails, the slower the scanning of video files is.
                 After deleting all duplicate videos, some additional matching ones may still be found by scanning again with a different thumbnail size.
pHash:           A fast and accurate algorithm for finding duplicate videos.
SSIM:            Even better at finding matches (less false positives especially, not necessarily more matches). Noticeably slower than pHash.
SSIM block size: A smaller value means that the thumbnail is analyzed as smaller, separate images. Note: selecting the value 2 will be quite slow.
Comparison       When comparing two videos, a comparison value is generated. If the value is below this threshold, videos are considered a match.
threshold:       A threshold that is too low or too high will either display videos that don't match or none at all.
Raise threshold: These two options increase/decrease the selected threshold when two videos have almost same length
Lower threshold: (meaning very likely that they match even if the computer algorithm does not think so).



Comparison window:
If matching videos are found, they will be displayed in a separate window side by side, with the thumbnail on top and file properties on bottom.
Clicking on the thumbnail will launch the video in the default video player installed.
Scrolling on the thumbnail with the mouse wheel will load a full size screen capture and zoom it, allowing a visual comparison of image quality,
Clicking on the filename in blue will open the file manager with the video file selected.
File properties are colour coded:
 - Tan: both videos have same property
 - Green: "better" property
 - Black: "worse" property (or not used)

Prev and next buttons: cycle backwards and forwards through all matching files.
Delete: Delete the video.
Move: Move the video to folder of opposite side.
Swap filenames: Change filenames between videos.

Beware that a poor quality video can be encoded to seem better than a good quality video.
Trust your eyes, watch both videos in a video player before deleting.



Vidupe Copyright (C) 2018, 2019 Kristian Koskim�ki
Vidupe is a free software distributed under the GNU GPL.
Read LICENSE.txt for more information.

![](http://i68.tinypic.com/ei8jza.jpg)
![](http://i64.tinypic.com/fy1ycw.jpg)