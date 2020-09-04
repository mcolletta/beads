# Changelog

## 3.2 - In Progress

### **Added**

* Users are now able to designate what type of data structure they want to use for storing and retrieving UGens
    * ie. Choice between ArrayLists or LinkedLists
    * UGens will use ArrayLists by default, if nothing is declared
* CrossFade Loop for LoopType.FINE has been added to SamplePlayer (Requires Further Testing)
    * Users must set a loop start and loop end point for crossfade to work
    * CrossFade available for forward, backward and alternating loops
    * Crossfade length cannot be less than 0, and if the user sets a value that is too large, it will automatically use the largest allowable length

### **Changed**

* Implementation has been changed to support JAudioLibs v2 (Released 18/8/20)
    * Modules effected: AudioServer Javasound & AudioServer JACK
* Licensing has been corrected: from Apache -> GPL3
* Processing Build has now been reverted to a thin package, showing all external libraries inside the /libs folder
* Default Audio Contexts have been updated
    * Refer to examples (Processing/examples or src/beads_tutorials) for how to use this. 

## 3.1 (Stable) - 23/7/2020

### **Added**

* Experimental CrossFade Loop has been added to SamplePlayer
    * Users must set a loop start point and a loop end point for crossfade to work.
* Instructions in the README file for setting up Maven or Gradle dependencies.

### **Fixed**

* Build.gradle for Maven Beads Distribution (v3.1) has been fixed to properly manage and locate dependencies now.

## 3.0  - 9/7/2020

### **Changed**

* Processing library build has now been flattened
* Build.gradle can now upload subsequent releases to Sonatype OSSRH
    * Credentials are stored in the .gradle folder seperate from this project.