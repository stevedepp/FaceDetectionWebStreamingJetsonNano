Thank you for watching my video.

I've had a chance to interact with 4 edge devices so far: Raspberry Pi4, Intel Neural Stick2, AWS DeepLens, and Jetson Nano.  I had never before spent any time with this type of device, and each time is a totally new kind of learning experience.  Throughout the last 7 weeks, I've been asking myself: what is this course about?  We don't actually spend much time using intense convolutional networks; so, how is this ComputerVision? 

Working with the Jetson Nano and to a lesser extend the Raspberry Pi over the last 3-4 days, it has dawned on me what I am learning and why it is useful.  It is very much similar to what I gained from Dr Miller's NLP course.  In MSDS 453 we spent the first couple weeks scraping data from the web.  It was an equally odd learning experience, but in the end very essential. 

Without the ability to scrape text from the internet, you cannot independently study NLP.  You will always be dependent on someone else to hand you a corpus. 

Similarly, without the ability to grab visual data, from edge devices, we cannot perform CV without someone handing us video or a collection of images.  So for me it is absolutely essential to learn as many ways to collect data from mobile edge devices that have cameras attached. 

I have found that the real challenge in this regard is power.  If you are collecting data with an edge device, it is likely on some battery power and getting it the right power quantity and type is key.  

This week, I have mastered power on the Nano and the Pi and come very close to vanquishing the cameras associated with both units as well. 

 

Will just link to the sources of the code:

I ssh into a headless battery powered Jetson Nano and call web_stream.py which broadcast back to my MBPro's browser the live video from the Jetson's Raspberry Pi camera.  Here's the code for web_stream.py

https://maker.pro/nvidia-jetson/tutorial/streaming-real-time-video-from-rpi-camera-to-browser-on-jetson-nano-with-flask (Links to an external site.)

I cloned this GitHub repository from JetsonHacks, a supremely useful and humorous resource for Jetson.  I attach an old HDMI monitor to the Jetson and run face_detect.py on a live video of my face and photos I hold up. Other than collecting the video specs, face_detect.py is only a few lines of code.  I spent a day trying to figure out how to integrate web_stream.py and face_detect.py so that I can stream back to my MacBookPro the face detection running on a battery powered Nano.   

https://github.com/JetsonHacksNano/CSI-Camera (Links to an external site.)

