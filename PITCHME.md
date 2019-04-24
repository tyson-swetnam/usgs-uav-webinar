---?image=https://media.giphy.com/media/orVa44Oav5WoF1LVOE/giphy.gif
<span style="font-weight: bold; font-size: 170%; color:#FFFFFF">Droning on about sUAS data pipelines, processing, and reproducible research</span> 
#### April 25, 2019
### Tyson Lee Swetnam Ph.D.
<img src="assets/imagery/cyverse_white.png" width="500">
+++

### My Contact Info

email: tswetnam@cyverse.org

github id: [tyson-swetnam](https://github.com/tyson-swetnam) & [cyverse-gis](https://github.com/cyverse-gis)

twitter: @tswetnam

talk link: https://github.com/tyson-swetnam/usgs-uav-webinar/ 

---?image=http://tile.loc.gov/image-services/iiif/service:gmd:gmd433:g4333:g4333p:la000006/full/pct:25/0/default.jpg
<span style="font-size: 300%; color:#000000">TODAY's ROADMAP </span>

+++

<span style="font-size: 150%; color:#FF0000"> 1) What's the big deal about sUAS? </span> <!-- .element: class="fragment" -->

<span style="font-size: 150%; color:#58FF33"> 2) Big Data ≠ Science (?) </span> <!-- .element: class="fragment" -->

<span style="font-size: 150%; color:#F9FF33"> 3) Processing sUAS data in cyberinfrastructure  </span> <!-- .element: class="fragment" -->

+++

<span style="font-size: 200%; color:#FF0000"> Do all the things </span>

<img src="http://rank-all-the-things.herokuapp.com/images/all_the_things.png" height="300"> 

---?image=https://media.giphy.com/media/ZNKTKocoj8e973Wptz/giphy.gif
## sUAS = AWESOME!

+++
![Video](https://www.youtube.com/embed/YpNIWaFXQs4)
+++
![Video](https://www.youtube.com/embed/xgNtQymN5GQ)
+++
![Video](https://www.youtube.com/embed/c1_yFK5jYC8)
+++
<img src="https://raw.githubusercontent.com/tyson-swetnam/srer-wgew/master/img/sensors.jpg" width="900"> 
+++
http://calliope.cyverse.org/pointclouds/casa_angelica/casa-angelica.html
+++

# PRO

<span style="font-size: 100%; color:#FF0000"> Ultra High Spatial Resolution </span> <!-- .element: class="fragment" -->

<span style="font-size: 100%; color:#58FF33"> Frequent Temporal Return Interval </span> <!-- .element: class="fragment" -->

<span style="font-size: 100%; color:#F9FF33"> Cheap </span> <!-- .element: class="fragment" -->

---?image=https://media.giphy.com/media/l0HlDHQEiIdY3kxlm/giphy.gif
## sUAS = PTSD

---?image=assets/imagery/firefly6_crash2.jpg
---?image=assets/imagery/firefly_crash1.jpg
+++
![Video](https://www.youtube.com/embed/RRc5LDJrk3I)
+++
![Video](https://www.youtube.com/embed/2_FD94RgLPE)
+++

# CON 

<span style="font-size: 100%; color:#FF0000"> Difficult to build and fly </span> <!-- .element: class="fragment" -->

<span style="font-size: 100%; color:#58FF33"> Needs integration across systems (Camera, RTK GNSS, lidar, etc) </span> <!-- .element: class="fragment" -->

<span style="font-size: 100%; color:#F9FF33"> Big Data → Requires massive computer processing </span> <!-- .element: class="fragment" -->

+++

## sUAS pilot = new profession

![Video](https://www.youtube.com/embed/IklFgsnGG0c)

+++

## Big Data: useless or transformative?

[How big data has created a crisis in Science](https://www.realclearscience.com/articles/2018/12/24/how_big_data_has_created_a_big_crisis_in_science_110838.html)

<span style="font-size: 150%; color:#F9FF33"> "Big Data ≠ Science" </span> 

<span style="font-size: 80%; color:#FF0000"> -- Anonymous Senior USGS Researcher </span>

+++

<img src="http://mattturck.com/wp-content/uploads/2018/07/Matt_Turck_FirstMark_Big_Data_Landscape_2018_Final.png" width="900">

@snap[south] Source: Matt Turck, 2018, http://mattturck.com 
@snapend

+++

<span style="font-size: 100%; color:#F9FF33"> Big Data </span>
    <span style="font-size: 80%; color:#FF0000"> (Binary & Unstructured) </span>
        <span style="font-size: 100%; color:#FFFFFF"> = "Level 0" data product </span>

<span style="font-size: 100%; color:#FFFFFF"> Process it <!-- .element: class="fragment" --> <span style="font-size: 100%; color:#F9FF33"> → Structured Data <!-- .element: class="fragment" --> 

+++

<span style="font-size: 100%; color:#F9FF33"> Structured Data </span>
    <span style="font-size: 80%; color:#FF0000"> (e.g. Imagery w/ metadata, Flight Logs, GPS Locations ) </span>
        <span style="font-size: 100%; color:#FFFFFF"> = "Level 1" data product </span>

<span style="font-size: 100%; color:#FFFFFF"> Index it <!-- .element: class="fragment" --> <span style="font-size: 100%; color:#F9FF33"> → Find, Search, Query <!-- .element: class="fragment" --> 
    
<span style="font-size: 100%; color:#FFFFFF"> Process it <!-- .element: class="fragment" --> <span style="font-size: 100%; color:#F9FF33"> → Information <!-- .element: class="fragment" --> 

+++

<span style="font-size: 100%; color:#F9FF33"> Information </span>
    <span style="font-size: 80%; color:#FF0000"> (e.g. Classified layers w/ metadata) </span>
        <span style="font-size: 100%; color:#FFFFFF"> = "Level 2-3" data product </span>

<span style="font-size: 100%; color:#FFFFFF"> Process it <!-- .element: class="fragment" --> <span style="font-size: 100%; color:#F9FF33"> → Knowledge <!-- .element: class="fragment" --> 

+++

<span style="font-size: 100%; color:#F9FF33"> Knowledge </span>
    <span style="font-size: 80%; color:#FF0000"> (Process, Mechanism) </span>
        
<span style="font-size: 100%; color:#FFFFFF"> Process it <!-- .element: class="fragment" --> <span style="font-size: 100%; color:#F9FF33"> → Judgement & Decision Making <!-- .element: class="fragment" --> 

---?image=https://media.giphy.com/media/uKpWZU3VXLprW/giphy.gif
<span style="font-weight: bold; font-size: 200%; color:#FFFFFF"> MOVING YOUR RESEARCH ONTO CYBERINFRASTRUCTURE </span>

+++

*different OS + third party software + updates/upgrades + redeployment* → 
 <span style="font-weight: bold; font-size: 100%; color:#FF0000">_Dependency Hell_ </span> 
 
<img src="https://imgs.xkcd.com/comics/python_environment_2x.png" height="400"> <!-- .element: class="fragment" --> <img src="https://pbs.twimg.com/media/DB6QcoNVYAA-w6N.jpg" height="400"> <!-- .element: class="fragment" -->

 <span style="font-weight: bold; font-size: 50%; color:#FF0000"> Source: XKCD.com, E. Dolstra 2006 https://nixos.org/~eelco/pubs/phd-thesis.pdf </span> 

---?image=https://media.giphy.com/media/GkQBupPcf5b1e/giphy.gif
<span style="font-weight: bold; font-size: 250%; color:#FFFFFF"> NOT YOUR LAPTOP OR DESKTOP </span>

+++ 

## Solution: Containerize software, run it anywhere. 

<img src="assets/imagery/ocelote.jpg" height="230">  <img src="https://cdn-images-1.medium.com/max/1600/1*yo62B91F4V1QIJYirBbxlQ.jpeg" height="230"> 

+++

## Why Containerize?

- Dependencies turn into wicked problems <!-- .element: class="fragment" -->
- Compiling software is sloooowww <!-- .element: class="fragment" -->
- Reproducibility is hard across platforms <!-- .element: class="fragment" -->
- Portability <!-- .element: class="fragment" --> **& _Scalability_** <!-- .element: class="fragment" -->

<img src="assets/imagery/vertical_large.png" width="200"> 

+++

### Deciding which UAV processing and analysis software to use?
<img src="assets/imagery/dreaming.png" width="500">

+++

<img src="https://pbs.twimg.com/media/Czf37xpWIAIc1-M.jpg" height="75">
<img src="https://www.integraldrones.com.au/wp-content/uploads/2016/06/Drone-deploy-image-2.jpg" height="75">
<img src="http://store.jdrones.com/v/vspfiles/photos/swpix4dpro01-2.jpg" height="75">
<img src="https://droneparts.de/media/image/fb/bb/03/Metashape_logo_.jpg" height="75">
<img src="https://uasweekly.com/wp-content/uploads/2017/06/Flyt-base-logo-1-copy.jpg" height="75">
<img src="https://d3pcsg2wjq9izr.cloudfront.net/files/51634/images/1.FarmersEdge-400.png" height="75">
<img src="http://jttaylor.net/gis/drone2map/images/drone2map-icon.jpg" height="75">
<img src="http://www.customerbliss.com/wp-content/uploads/2016/06/Esri-Logo-Compact.png" height="75">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c2/QGIS_logo%2C_2017.svg/1280px-QGIS_logo%2C_2017.svg.png" height="75">

<img src="https://www.logolynx.com/images/logolynx/11/11176029fe5b1cb338bc7cc437aee68d.png" height="75">
<img src="https://nordicapis.com/wp-content/uploads/Azure-logo.png" height="75">
<img src="http://www.thatlazyadmin.com/wp-content/uploads/2017/09/google-cloud-logo.png" height="75">

+++

## Working with sUAS data in Cyberinfrastructure

<img src="assets/imagery/calliope_logo.png" width="400">

+++

<img src="assets/imagery/sUAS_pipeline.jpg" width="1200">

+++

<img src="assets/imagery/workflow_calliope_clowder.png" width="1200">

---?image=https://media.giphy.com/media/wUCgLRvDdtWs8/giphy.gif
# Have Workflow, Will Travel

+++

<img src="assets/imagery/SfM-MVS-Clowder.jpg" width="1200">

+++

<span style="font-weight: bold; font-size: 150%; color:#FF0000">Graphical User Interfaces </span>
 
- Need more computing power than a laptop </span>
- Cannot afford to buy a $5,000 workstation </span>

---?image=assets/imagery/dockerhub_ubuntu_xfce.png

---?image=assets/imagery/metashape.jpg

+++

<span style="font-weight: bold; font-size: 150%; color:#F0FF00"> Power Users </span>

- Interest in scaling workflow beyond the laptop / desktop onto HPC and Cloud </span>
- Need to run 10s to 1,000s of jobs (sUAS flights) across a large geographic area </span>

---

### The "Bring Your Own Data" Approach

<img src="assets/imagery/cyverse_white.png" width="800">

+++

### Important: CyVerse is enabled by 

<span style="font-weight: bold; color: #c7232e">_People & Research Objectives_</span> 

### Success depends on users innovating within an ecosystem of interoperability  <!-- .element: class="fragment" -->

+++

<img src="http://www.twincities.com/wp-content/uploads/2015/11/20130102__field-of-dreamsl.jpg" height="250"> <img src="https://theamericangenius.com/wp-content/uploads/2014/02/field-of-dreams.jpg" height="250">

<span style="font-weight: bold; font-size: 200%; color:#FF0000"> NOT! </span> <!-- .element: class="fragment" -->

+++

### In CyVerse <span style="font-weight: bold; color: #3685E3">_we work with you_ </span> to identify the tools, workflows, and datasets you need.

<img src="http://insidethegem.com/wp-content/uploads/organic-logo.png" height="150"> <img src="http://cstaab.com/wp-content/uploads/cpp_java_python.png" height="150"> <img src="https://pbs.twimg.com/profile_images/662507863516905472/7piKPHHv_400x400.jpg" height="150"> 

+++

## [Atmosphere](https://cyverse.org/atmosphere)

<img src="assets/imagery/Atmosphere_white.png" width="200">

### On demand cloud computing for scientific research

+++

<img src="assets/imagery/Atmosphere_white.png" width="200">

- Linux environment (CentOS, Ubuntu)
- Collaborate together online
- Publicly host custom images

+++

<img src="assets/imagery/Atmosphere_white.png" width="200">

- Multiple instance sizes and 'flavors'
  - 1 CPU, 4GB RAM, 30GB Disk
  up to 
  - 16 CPU, 128GB RAM, 1400GB Disk
- Attach (and swap) external storage volumes    
- emulated web shell and desktop via [ApacheGuacamole](https://guacamole.incubator.apache.org/)  

+++

<img src="https://raw.githubusercontent.com/OpenDroneMap/OpenDroneMap/master/img/odm_image.png" height="150">

```shell
$ ezd
$ sudo docker run -d -p 3000:3000 opendronemap/node-opendronemap
Done!
```

@[1](install Docker)
@[2](Run the Container)
@[3](Open the Node OpenDroneMap in a new browser tab on the VM IP on port :3000)

+++

## [Discovery Environment](https://de.cyverse.org)

<img src="assets/imagery/Discovery_white.png" height="200">

A Data Science Workbench

+++

<img src="assets/imagery/Discovery_white.png" height="200">

- Add your own Docker containers as "Tools"
- Build "Apps" with interfaces for users (equivalent command-line interface execution)
- Create a sequenced workflow by chaining one app to another in an automated workflow.

+++

### Visual Interactive Computing Environment (VICE)

<img src="assets/imagery/vice.png" width="400">

Work with your data interactively in your favorite IDE

+++

<img src="assets/imagery/vice_diagram_small.png" width="800">

---

### Host and Publish Data

---?image=assets/imagery/gillan_etal.png

+++

[link](http://datacommons.cyverse.org/browse/iplant/home/shared/commons_repo/curated/Gillan_et_al_RAMA_2019)

+++

### [DataCommons](http://datacommons.cyverse.org/)

<img src="assets/imagery/DataCommons_White.png" height="200">

- Share data with community members & public
- "CyVerse Curated" → DOI
- "Community Released" → living & shared

---

### Data Transfer

- iRODS iCommands (CLI)
- WebDav (HTTPS)
- Discovery Environment 
- CyberDuck

---

## Why are we focused on automating this stuff?

<span style="font-size: 100%; color:#F9FF33"> Good programmers are hard working. <!-- .element: class="fragment" --> 
    
<span style="font-size: 100%; color:#FF0000"> Great programmers are lazy. <!-- .element: class="fragment" --> 

+++

[Alan Perlis, 1982 Epigrams on Programming](https://web.archive.org/web/19990117034445/http://www-pu.informatik.uni-tuebingen.de/users/klaeren/epigrams.html)

**54. Beware of the Turing Tarpit in which everything is possible but nothing of interest is easy.**

<img src="https://img00.deviantart.net/58af/i/2012/093/a/c/la_brea_tar_pits_by_felipenn-d4uxy05.jpg" width="400">

+++

### Building the "best" workflows and pipelines takes time and experience

<img src="https://d13ezvd6yrslxm.cloudfront.net/wp/wp-content/images/edgeoftomorrow-livedierepeat-cruise-blunt-postercrop.jpg" width="800">

+++

### Getting stuff done.

<span style="font-size: 100%; color:#FF0000"> 1) Do the things. <!-- .element: class="fragment" -->
<span style="font-size: 120%; color:#F9FF33"> → 2) Do the things right. <!-- .element: class="fragment" -->
    
<span style="font-size: 200%; color:#58FF33"> → 3) Do the things well. <!-- .element: class="fragment" -->

+++

### Want to learn more about programming?

<img src="https://carpentries.org/images/TheCarpentries-opengraph.png" width="800">

https://carpentries.org

+++

### Want to learn more about CyVerse?

Focus Forum Webinars: https://www.cyverse.org/ffw

+++

### [The Learning Center](http://learning.cyverse.org/en/latest/) 

<img src="assets/imagery/Learningcenter_white.png" height="200"> 

http://learning.cyverse.org/en/latest/

+++

### Upcoming event: Foundational Open Science Skills (FOSS)
#### June 3–14, 2019
##### Location: University of Arizona, Tucson AZ

https://www.cyverse.org/foss

<img src="https://static.wixstatic.com/media/1f832b_cbc41b96ceab44298f7522fa7ad9b7fe~mv2.jpg" width="800">

---

## Acknowledgments

GIFs by Giphy.com

All digital images shown this presentation are available online and are the property of their creators, their web addresses are visible in the source code of this presentation at: https://github.com/tyson-swetnma/usgs-uav-weibnar/PITCHME.md 

---?image=assets/imagery/endslide.png
