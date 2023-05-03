# BrainBraille-Spring-2023
Created a Minimum Viable Product that enables users to learn BrainBraille quickly and get prepared for an fMRI environment.

Follow this guide for installing and setting up OpenPose: https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md#windows-portable-demo. On Windows Machines, install v 1.16.0 which is the version right before the latest version.

For running on live video, you can run the following command:

../openpose.bin --face --hand

where ".." represents the directory that your openpose.bin file is located in. For our purposes, since we created an Minimum Viable Product (MVP), there is no need to run the face library especially because it will simply slow things down and isn't particularly useful unless a second camera is set up exclusively for the user's face.

../openpose.bin --hand

Other tags we used were --tracking, number_people_max, write_video, and write_video_fps. By reducing the accuracy a little, the speed of the OpenPose can be improved significantly. We used --tracking 5, meaning every 5 frames instead of tracking every frame (--tracking 0, which is the default). We set number_people_max to 1 since we were only testing on 1 person at a time. For write_video, we gave the path that we wanted to write our video to ("../path/video.avi") and for write_video_fps we made sure our video was 5 fps with write_video_fps 5 so that the video was fairly easily followable.

For other commands, please refer to the following link:
https://cmu-perceptual-computing-lab.github.io/openpose/web/html/doc/index.html

For the virtual reality component, the code can be edited and ran on WebVR/VR mode on Glitch.com.

Here is the link to be able to view/edit the code ... https://glitch.com/edit/#!/resilient-berry-broker .
Otherwise, the main bulk of the code has been uploaded to the index.html file.

To run it on the BNext VR Headset, or any headset with a phone tray holder, click share on the website and use the livesite link to pull it up on the device you use. Be sure to click "VR Mode"
