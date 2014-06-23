# Sharethrough "Meaningful Content Website" Frontend Interview Test
This test is way to gauge your frontend skills.  Specifically this test should measure your knowledge and experience with the following:
* LESS
* Bootstrap 3
* CSS3
* HTML5
* jQuery/Javascript
* Rails

#### Table of Contents
- [Basic Rules](#rules)
- [Getting the Environment Set Up](#setup)
- [Scenario](#scenario)
- [Directions](#directions)
- [Submitting the Final Work](#submit)

## <a id="rules"></a>Basic Rules
You can use the Internet as a resource to answer any of the technical questions you may have - we want to simulate a real world environment as much as possible. This also is NOT meant to test your ability in setting up Rails, so if you a struggling to get the environment initially setup please contact the hiring manager.

The **[following PDF](../master/directions/MCF%20Responsive%20Mocks.pdf?raw=true)** is high-fidelity mock up of what the site should look like.  Each page of the PDF is a mocked up version of each responsive state.  So page 1 is the desktop site, page 2 is the tablet site and page 3 is the mobile site.  

The current site _mostly_ matches it except for a few responsive states.  It is also missing a video background and some jQuery snazziness.  The goal of this exercise is to have the site match the mock-up.  The directions below will go into more details.

You should use the frameworks as much as you can (versus coming up with your own CSS, HTML, or JS).  That said you will need to alter some of the existing code to make some of these steps work.

## <a id="setup"></a>Getting the Environment Set Up
Since the point of this exercise is to gauge your ability with the above listed frameworks/languages, we have provided step-by-step directions to getting the application installed and working as is.

1. Clone the repository from Github: ```git clone git@github.com:sharethrough/frontend-interview-test.git```
2. Install all the necessary requirements: ```bundle install```
3. Start up the app: ```rails s```
4. Visit: ```http://localhost:3000```

Again, if you are struggling to get this working, please contact the hiring manager.

## <a id="scenario"></a>Scenario
Sharethrough wants to create a new marketing site called Meaningful Content which highlights some of the best content that exists on the Internet. This site will be a stand alone website (separate from [sharethrough.com](http://sharethrough.com)) so it will be powered by its own database, design, etc.

FYI - the actual [live site](http://meaningfulcontent.org) has a different design and framework powering it, so you can use it as way to understand the purpose, but it isn't helpful to use the live site as a reference.

A base version of the site has been outsourced and we now need it make some changes and additions to it.

## <a id="directions"></a>Directions
There are a few tweaks that need to be made to the existing app.  Each task tests a different skill set and can be done independently of each other. This exercise should take no more than **2-3 hours** and if you find yourself spending more time than that please just submit what you have you accomplished at the end of that time.

### 1.  Making the Mobile Cards Look Right  (LESS, Bootstrap 3)
If you look at the mobile mock of the site (page 3 of the PDF), the titles on each of the "cards" should be overlayed on top of the image instead of below the image.  

**This change will only apply to the MOBILE responsive state of the site.**

| Current State | Desired State |
| ------------- | ------------- |
| ![mobile current](../master/directions/mobile%20cards%20before.png?raw=true) | ![mobile desired](../master/directions/mobile%20cards%20after.png?raw=true) |

### 2.  Tablet Nav Bar isn't as Designed  (LESS, Bootstrap 3)
The current tablet nav bar is just inheriting the desktop look and feel.  Please modify the nav bar for the tablet responsive state so that it matches the mock up.

**This change will only apply to the TABLET responsive state of the site.**

| Current State | Desired State |
| ------------- | ------------- |
| ![mobile current](../master/directions/tablet%20nav%20before.png?raw=true) | ![mobile desired](../master/directions/tablet%20nav%20after.png?raw=true) |

### 3.  Add a Video as the Background of the Site (HTML5)
We'd like to add a video to the background of the site, so that there is a subtle video auto-playing when a user hits the site.  The assets for the video can be found at _/app/assets/images/bg-vid.mp4_ and _/app/assets/images/bg-vid.png_.

**This change will apply to ALL responsive states of the site.**

![Video Background](../master/directions/video%20bg%20after.png?raw=true)
<br>*Video is very subtle, so it is hard to see, but obviously the background should be animated.

### 4.  Implement the Smooth Scroll jQuery Plugin (jQuery/Javascript)
Implement the [smooth scroll plugin](https://github.com/cferdinandi/smooth-scroll#readme) (already included and being loaded by the browser) so that clicking on the nav bar links will jump and smooth scroll to each corresponding section.

**This change will apply to ALL responsive states of the site.**

![Smooth Scroll](../master/directions/smoothscroll.gif?raw=true)

## <a id="submit"></a>Submitting the Final Work
When you have finished your work.  Please zip up the entire application folder and send the compressed folder to the hiring manager.  Make sure that what is zipped up contains all necessary files to run the application.
