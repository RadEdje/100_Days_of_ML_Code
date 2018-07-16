Day 0: July 7, 2018

Today's Progress: Saw Siraj's #100DaysOfMlCode on both FB and Twitter and finally decided to start this log and shared the 
link to the work I'm doing.

Intro: I started with google's crash course in machine learning about 1-2 months ago then went to tensorflow.js after I saw the amazing
demo for the emoji scavenger hunt. This is how my journey into AI/ML with tensorflow and tensorflow.js began.

About the APP: 
I'm building a web app that uses tensorflow.js to deploy an AI/ML model I trained. The app uses the web cam to scan an image and 
tries to detect monteggia and galeazzi fractures then produces a link with an image search for pictures on the web that look similar to the
scanned image. I'm basically shooting for a reverse image search using AI/ML deployed on the web with javascript.

latest iteration has just been updated to tensorflow.js version  0.11.7 and tensorflow (python version 1.8)

Thoughts:
After updating to the latest tf (python and javascript), model.predict() has become exceedingly fast on the web, way faster than with tf.js 
version 0.10.0. This has somehow affected the accuracy of my AI/ML model's predictions. Still exploring the reason.

Same problems with iOS devices. Minimum requirement on apple devices is still safari 11 (since this is the version that supports webRTC and
access to the web cam).

Android support is growing:
--current device support based on user feed back is samsung galaxy s8, galaxy a5, Mi6 and OnePlus 5t. (mostly android 7-8 devices).
--Still can't figure out why it won't work on android 5... last link/forum I found indicated a performance cliff...
https://github.com/tensorflow/tfjs/issues/145

Current problem:
Continue to figure out how to get it to work on older droids? 

or 

just continue to develop since I have more features to add like
DICOM support (hoping when I'm done with development, most droid will be on android 8.0)

Link to work: https://radhorizon.com/SITES/RadLense/index3.html

Day 2: July 9, 2018

Progress, still stuck with WebRTC for iOS safari 11. Can't initiate the camera for the app. Been trying to figure it out since yesterday.
Taking a break on that and reviewing YOLO and YOLO2 by watching SIRAJ's vid at
https://www.youtube.com/watch?v=4eIBisqx9_g
I wonder if tensorflow.js is now fast enough to do this on the web?

UPDATE: web app now working on iOS! Yahoo.... though though still not working on android 5 and lower (can't seem to get over the performance cliff....). Working mostly on android 7-8. Will work on UX and possible ideas of DICOM support.

DAY 3: July 10, 2018
Current Progress: 
Uploaded the latest version of the AI/ML web app and asking for feedback from users. The updates were focused mainly for iOS incompatibilities. I hope the changes don't break existing compatibilities with other android phones. Finger's crossed.

Current goals:
Hope to move forward with Either DICOM scanning or YOLO for the app. Must check if anyone has already successfully run YOLO in the browser of a mobile phone.

Current project link:
https://radhorizon.com/SITES/RadLense/index6.html

DAY 3: July 14, 2018

Got tied to work past couple of days.

Watching an intro to GAN (if I can use it in my web app).
https://www.youtube.com/watch?v=9JpdAg6uMXs

Also got an amazing link to https://deepcognition.ai/
first AI IDE with GUI drag n drop pluse terminal support for KERAS and TENSORFLOW.... can't wait to try it out...just waiting for
my slow internet to download.

DAY 4: July 16, 2018
Reviewing batch size, iterations and epochs for the new model web app I'm considering.
reading: https://towardsdatascience.com/epoch-vs-iterations-vs-batch-size-4dfb9c7ce9c9
https://www.quora.com/Intuitively-how-does-mini-batch-size-affect-the-performance-of-stochastic-gradient-descent


Current problem:
with my old data set of 200+ gray scale images, I could get considerable validation accuracy with a batch size of 2 and 15-17 epochs but after increasing my data set to 400+ colored images, I can't get passed 20--30% validation accuracy even after increasing my epochs to 30.

Possible solutions:
Might further increase the batch sizes. If  that does not work, I might have to adjust the learning rate (currently using ADAM optimier).
