[Anthill](http://www.anthill.com/) - Task Management Done Right
================================  
Anthill strives to be a simple and effective organization tool for Google Android phones. It comes with features like reminders, tagging, widgets, and integration with online synchronization services.

Interested in using Anthill? Search "Anthill" in Android Market. Look for the smiling pink squid!

If you would like to help out with the Anthill project, you're in the right place.

Getting Started With Development
---------------

1. Create your own fork of Anthill by clicking on Github's *Fork* button above (you may have to log in first - .

2. Install the following: 
 • *[git](http://git.or.cz/)*
 • *[Eclipse](http://eclipse.org)* (preferred: Eclipse IDE for Java Developers)
 • *[Android SDK](http://developer.android.com/sdk/index.html)* (Recommended SDK Platform: Android 4.0 Google APIs)
 • *[ADT Plugin for Eclipse](http://developer.android.com/sdk/eclipse-adt.html)*

3. Use **git** to clone your forked repositories 

`git clone git@github.com:yourgithubid/Anthill.git` 

(see Github's instructions if you need help). Follow the [Github Line Ending Help](http://help.github.com/dealing-with-lineendings/)

4. Open up **eclipse** and import the *anthill*, *anthillApi*, *anthill-tests*, *facebook*, and *GreenDroid* projects. 

5. In Eclipse preferences -> Android build settings, set the SDK location (you installed it in step 2). At this point, there should be no compilation errors. If there are, you might have to **refresh** and **clean** the projects a few times from within **eclipse** 

*from Eclipse: project-menu -> clean -> select projects -> check "start a build immediately" if "automatic build" is not enabled*

6. Launch the *anthill* project as an **Android Application**, or the *anthill-tests* project as an **Android JUnit Test Suite**.

7. Join the [Anthill Power-Users List](http://groups.google.com/group/anthill-power).

8. Check out the [Product Roadmap](http://wiki.github.com/todoroo/anthill/) and [Issues](http://github.com/todoroo/anthill/issues), and look for something you'd want to tackle.

9. Read the following contributor and debugging workflow and help make Anthill better!

10. Sign a [Contributors License Agreement](https://github.com/downloads/todoroo/anthill/Contributors%20Licensing%20Agreement.pdf) and send it to tim AT anthill.com 

Testing on a device - Debugging
---------------
How to debug/test on a USB device: (JoshuaGross Jan 14, 2011)

1. Plug in your device and make sure you can see it by running `adb devices`

2. If you cannot see the device, or want to restart debugging, do:

`adb kill-server`

`adb usb`

`adb devices` (make sure your device is listed)

`adb uninstall com.todoroo.anthill.tests` (you should see "Failure" if this was uninstalled already)

`adb uninstall com.todoroo.anthill` (you should see "Failure" if this was uninstalled already)

3. If you have not already, set up Run configurations in Eclipse; either under the "Run" or "Debug" menus. To test the application, set up "Android Application". To run JUnit tests, set up "Android JUnit Tests". Settings should autofill for you, you should be able to open a new configuration and run it. If you run it in debug mode, see #2 above for getting adb to work in case it is finicky.

4. When running unit tests: make sure to *close all JUnit windows* before running tests. JUnit/Eclipse/Android work together in a very, very janky way. You may get incorrect results if you do not close the window out before running tests. You have been warned.

5. Make sure to commit changes both to the "anthill" project while developing.

Contributors workflow
---------------

**Setup:**

`git clone git@github.com:your-github-id/Anthill.git` (your-github-id should obviously be replaced)

Contact
-------
For general support requests, use [Nmachi Ciaran](http://github.com/N-Ciaran).
