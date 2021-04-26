# Demo of live video face detection using webstream from a Jetson Nano

The audio for this demo video is available when you click on the image below, or you can follow the transcript and visuals that are just below the video.

Here are some significant [thoughts](https://github.com/stevedepp/FaceDetectionWebStreamingJetsonNano/blob/main/edge_device_importance.md) on the importance of edge devices in computer vision, with parallels to web scraping and NLP.

![demo](https://user-images.githubusercontent.com/38410965/111724301-64c4d000-883b-11eb-9546-555a324eaa9e.mp4)

#

> Hi. This is Steve. Thank you for watching my video.  I’ve had a decent amount of success over the last couple days with power management on both these units on the right.  One is the Raspberry Pi and the other is the Jetson Nano.  So, I’m able to operate them *mobilly* on battery power on a fairly reliable basis, and then in the last couple days, specifically today and late yesterday, I’ve had success getting getting web streaming from the Nano and getting face detection from the Nano, though not together, and I will show you what I mean here. 

<img width="1140" alt="image" src="https://user-images.githubusercontent.com/38410965/116126355-8f087980-a694-11eb-9c75-c364178343d4.png">

#

> So, I’ve just ssh’d into the Nano, ... 

<img width="1140" alt="image" src="https://user-images.githubusercontent.com/38410965/116126585-d0992480-a694-11eb-969a-df2363c19d99.png">

#

> ... and I’m going to use a web streaming function that I found on the internet and just sort of wrote up, here.  So, it runs on Python 3.  (Think it’s `py`.)  And then it broadcasts into a web browser.  OK. So, I’m upside down there.  That was kind of intentional actually.  I’ll be able to fix that, but I wanted to show you the fix.  So, while that’s fixing, I’ll have to actually restart the Nano, and while that’s doing that, I will show you a quick video of what else I’ve done.

 `python3 webstream.py`

<img width="1140" alt="image" src="https://user-images.githubusercontent.com/38410965/116126689-f292a700-a694-11eb-819b-f3377dd97e39.png">

#

> So, in this video, I actually had to load up, err, or attach a monitor to Nano, which wasn’t really my preferred way of doing it, but I couldn’t figure out a way to get the video over to my MacBook from the Nano as it did face detection.  And I’ll show you this program here in just a minute. The code is relatively short and is written by a fellow who has a YouTube account called Jetson Hacks.  He’s quite good and very helpful.  

<img width="1140" alt="image" src="https://user-images.githubusercontent.com/38410965/116126992-4ac9a900-a695-11eb-8787-938afd1b8bb8.png">

<img width="1140" alt="image" src="https://user-images.githubusercontent.com/38410965/116127264-a136e780-a695-11eb-9f71-204d5393803c.png">

#

> *(In the demo video, I’m doing two things at this point: re-powering the Nano and commenting on another video I created.)*

> Anyway. So, in this video, I am just using this face detection routine.  *(Let’s see if we are back in.)*  You can see it just operating.  

<img width="1140" alt="image" src="https://user-images.githubusercontent.com/38410965/116127441-d7746700-a695-11eb-8f9f-0d3e8f25659e.png">

#

> There. So, you can see it’s picking up faces of, this is actually me when I was a little kid, from a photograph, ...

<img width="1140" alt="image" src="https://user-images.githubusercontent.com/38410965/116127710-27ebc480-a696-11eb-85ea-87d4653e8b26.png">

#

> ... and then on the other side, I’ll show you how it picks up my wife and I.  It’ll pick up our eyes fairly reliably.  On the left hand side here is the extent of the program.  So, you’ll see it’s really a short program.  Kind of amazing.  Most of it, in fact, most of it is just variable retrieval. So, I’ll get out of this, and we’re done with that.  

<img width="1140" alt="image" src="https://user-images.githubusercontent.com/38410965/116127784-3934d100-a696-11eb-9b95-c6fd9c62680a.png">

# 

> So, I will now go into the other one *(the live demo of the Nano after it is re-powered)*, and change the setting so that I’m right side up. That’s `web stream dot py`.  So, in this, we’re able to change all sorts of aspects of how the video is retrieved and broadcast, (`flip-method=0` --> `flip-method=2`), which really is useful because essentially what we’re trying to do is get good data, and unless we’re able to manipulate it, we won’t be able to get good data.  

`flip-method=0`

<img width="602" alt="image" src="https://user-images.githubusercontent.com/38410965/116128454-f9221e00-a696-11eb-84f5-d6a297afe2be.png">

`flip-method=2`

<img width="600" alt="image" src="https://user-images.githubusercontent.com/38410965/116128735-41414080-a697-11eb-9ea3-644ad6192439.png">

#

> Here we go.  I’ll try and see if I can do that again. What is it? It’s `python3 webstream.py`, and with any success, I will be right side up.  There you go!  Thank you again for watching.    

<img width="1140" alt="image" src="https://user-images.githubusercontent.com/38410965/116128214-b3655580-a696-11eb-938b-207e677f172f.png">



