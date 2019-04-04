---

<span style="font-weight: bold; font-size: 170%; color:#FFFF00">Droning on about sUAS data pipelines, processing, and reproducible research</span> 

April 5, 2019
#### Tyson Lee Swetnam Ph.D.
<img src="assets/imagery/cyverse_white.png" width="500">

+++

### Contact Info

email: tswetnam@cyverse.org

github id: [tyson-swetnam](https://github.com/tyson-swetnam) & [cyverse-gis](https://github.com/cyverse-gis)

twitter: @tswetnam

talk link: https://github.com/cyverse-gis/uav-webinar/ 

---

# Today's Roadmap

+++

<span style="font-size: 100%; color:#58FF33"> 1) Work with sUAS data in cyberinfrastructure </span> <!-- .element: class="fragment" -->

<span style="font-size: 100%; color:#F9FF33"> 2) Reproducible techniques for data processing & data management </span> <!-- .element: class="fragment" -->

<span style="font-size: 150%; color:#FF0000"> Do all the things </span> <!-- .element: class="fragment" -->

<img src="http://rank-all-the-things.herokuapp.com/images/all_the_things.png" height="300"> <!-- .element: class="fragment" -->

---

## Big Data: useless or transformative?

[How big data has created a crisis in Science](https://www.realclearscience.com/articles/2018/12/24/how_big_data_has_created_a_big_crisis_in_science_110838.html)

<span style="font-size: 150%; color:#F9FF33"> "Big data ≠ science" </span> <!-- .element: class="fragment" -->

<span style="font-size: 80%; color:#FF0000"> -- Anonymous senior-researcher </span> <!-- .element: class="fragment" -->

---?image=http://mattturck.com/wp-content/uploads/2018/07/Matt_Turck_FirstMark_Big_Data_Landscape_2018_Final.png

Source: Matt Turck, 2018, http://mattturck.com

+++

![image](https://upload.wikimedia.org/wikipedia/commons/thumb/9/94/Gartner_Hype_Cycle.svg/1000px-Gartner_Hype_Cycle.svg.png)

Source: Wikipedia, Gartner Inc. Hype Cycle
+++

<span style="font-size: 100%; color:#F9FF33"> Big Data <!-- .element: class="fragment" --> 
    <span style="font-size: 80%; color:#FF0000"> (Binary & Unstructured) <!-- .element: class="fragment" --> 
        <span style="font-size: 100%; color:#FFFFFF"> = "Level 0" data product <!-- .element: class="fragment" --> 

<span style="font-size: 100%; color:#FFFFFF"> Process it <!-- .element: class="fragment" --> <span style="font-size: 100%; color:#F9FF33"> -> Structured Data <!-- .element: class="fragment" --> 

+++

<span style="font-size: 100%; color:#F9FF33"> Structured Data <!-- .element: class="fragment" --> 
    <span style="font-size: 80%; color:#FF0000"> (e.g. Imagery w/ metadata, Flight Logs, GPS Locations ) <!-- .element: class="fragment" --> 
        <span style="font-size: 100%; color:#FFFFFF"> = "Level 1" data product <!-- .element: class="fragment" --> 

<span style="font-size: 100%; color:#FFFFFF"> Process it <!-- .element: class="fragment" --> <span style="font-size: 100%; color:#F9FF33"> -> Information <!-- .element: class="fragment" --> 

+++

<span style="font-size: 100%; color:#F9FF33"> Information <!-- .element: class="fragment" --> 
    <span style="font-size: 80%; color:#FF0000"> (e.g. Classified layers w/ metadata) <!-- .element: class="fragment" --> 
        <span style="font-size: 100%; color:#FFFFFF"> = "Level 3" data product <!-- .element: class="fragment" --> 

<span style="font-size: 100%; color:#FFFFFF"> Process it <!-- .element: class="fragment" --> <span style="font-size: 100%; color:#F9FF33"> -> Knowledge <!-- .element: class="fragment" --> 

+++

<span style="font-size: 100%; color:#F9FF33"> Knowledge <!-- .element: class="fragment" --> 
    <span style="font-size: 80%; color:#FF0000"> (Process, Mechanism) <!-- .element: class="fragment" --> 
        
<span style="font-size: 100%; color:#FFFFFF"> Process it <!-- .element: class="fragment" --> <span style="font-size: 100%; color:#F9FF33"> -> Judgement & Decision Making <!-- .element: class="fragment" --> 

+++

## Pitfalls while working in bespoke software and environments

+++

*different OS + third party software + updates/upgrades + redeployment* = 
 <span style="font-weight: bold; font-size: 100%; color:#FF0000">_Dependency Hell_</span> <!-- .element: class="fragment" -->
 
<img src="https://imgs.xkcd.com/comics/python_environment_2x.png" height="400"> <!-- .element: class="fragment" --> <img src="https://pbs.twimg.com/media/DB6QcoNVYAA-w6N.jpg" height="400"> <!-- .element: class="fragment" -->

Source: XKCD.com, E. Dolstra 2006 https://nixos.org/~eelco/pubs/phd-thesis.pdf 

+++ 

## Solution: Containerize software, run it anywhere. 

<img src="https://cdn-images-1.medium.com/max/1600/1*yo62B91F4V1QIJYirBbxlQ.jpeg" width="400"> <!-- .element: class="fragment" -->

+++

## Why Containerize?

- Dependencies turn into wicked problems <!-- .element: class="fragment" -->
- Compiling software is sloooowww <!-- .element: class="fragment" -->
- Reproducibility is hard across platforms <!-- .element: class="fragment" -->
- Portability <!-- .element: class="fragment" --> **& _Scalability_** <!-- .element: class="fragment" -->

+++

### Deciding which UAV processing and analysis software to use?
<img src="assets/imagery/dreaming.png" width="500">

+++

<img src="https://pbs.twimg.com/media/Czf37xpWIAIc1-M.jpg" width="150">
<img src="https://www.integraldrones.com.au/wp-content/uploads/2016/06/Drone-deploy-image-2.jpg" width="150">
<img src="http://store.jdrones.com/v/vspfiles/photos/swpix4dpro01-2.jpg" width="150">
<img src="https://droneparts.de/media/image/fb/bb/03/Metashape_logo_.jpg" width="150">
<img src="https://uasweekly.com/wp-content/uploads/2017/06/Flyt-base-logo-1-copy.jpg" width="150">
<img src="https://d3pcsg2wjq9izr.cloudfront.net/files/51634/images/1.FarmersEdge-400.png" width="150">

<img src="https://www.logolynx.com/images/logolynx/11/11176029fe5b1cb338bc7cc437aee68d.png" width="150">
<img src="https://nordicapis.com/wp-content/uploads/Azure-logo.png" width="150">
<img src="http://www.thatlazyadmin.com/wp-content/uploads/2017/09/google-cloud-logo.png" width="150">

+++


[Alan Perlis, 1982 Epigrams on Programming](https://web.archive.org/web/19990117034445/http://www-pu.informatik.uni-tuebingen.de/users/klaeren/epigrams.html)

**54. Beware of the Turing Tarpit in which everything is possible but nothing of interest is easy.**

<img src="https://img00.deviantart.net/58af/i/2012/093/a/c/la_brea_tar_pits_by_felipenn-d4uxy05.jpg" width="400">

+++

### Building the "best" workflows and pipelines takes time and experience

<img src="https://d13ezvd6yrslxm.cloudfront.net/wp/wp-content/images/edgeoftomorrow-livedierepeat-cruise-blunt-postercrop.jpg" width="800">

+++

<img src="assets/imagery/sUAS_pipeline.jpg" width="1200">

+++

<img src="assets/imagery/workflow_calliope_clowder.png" width="1200">

---

## Have Workflow, Will Travel

<img src="https://rhystranter.files.wordpress.com/2016/11/studio-ghibli-howls-moving-castle.jpg" height="400">

+++

## Why are we focused on automating this stuff?

<span style="font-size: 100%; color:#F9FF33"> Good programmers are hard workin g. <!-- .element: class="fragment" --> 
    
<span style="font-size: 100%; color:#FF0000"> _Great_ programmers are lazy. <!-- .element: class="fragment" --> 

+++

## Working with sUAS data in Cyberinfrastructure

<img src="assets/imagery/calliope_logo.png" width="400">

+++

<img src="assets/imagery/SfM-MVS-Clowder.jpg" width="1200">

+++

<span style="font-weight: bold; font-size: 150%; color:#FF0000">Graphical User Interfaces</span>
 
- Need more computing power than a laptop <!-- .element: class="fragment" -->

- Cannot afford to buy a $5,000 workstation <!-- .element: class="fragment" -->

---?image=assets/imagery/dockerhub_ubuntu_xfce.png

---?image=assets/imagery/metashape.jpg
+++

<span style="font-weight: bold; font-size: 150%; color:#F0FF00">Power Users</span>

- Interest in scaling workflow beyond the laptop / desktop onto HPC and Cloud <!-- .element: class="fragment" -->

---

### Working with your data in CyVerse

+++

### Important: CyVerse is enabled by <span style="font-weight: bold; color: #c7232e">_People & Research Objectives_</span>  <!-- .element: class="fragment" -->

### Our success depends on users innovating within an ecosystem of interoperability  <!-- .element: class="fragment" -->

+++

<img src="http://www.twincities.com/wp-content/uploads/2015/11/20130102__field-of-dreamsl.jpg" height="250"> <img src="https://theamericangenius.com/wp-content/uploads/2014/02/field-of-dreams.jpg" height="250">

<span style="font-weight: bold; font-size: 150%; color:#FF0000">NOT!</span> <!-- .element: class="fragment" -->

+++

### In CyVerse <span style="font-weight: bold; color: #3685E3">we work with you</span> to identify the tools, workflows, and datasets you need.

<img src="http://insidethegem.com/wp-content/uploads/organic-logo.png" height="150"> <img src="http://cstaab.com/wp-content/uploads/cpp_java_python.png" height="150"> <img src="https://pbs.twimg.com/profile_images/662507863516905472/7piKPHHv_400x400.jpg" height="150"> 

+++


## [Atmosphere](https://cyverse.org/atmosphere)

<img src="assets/imagery/Atmosphere_white.png" width="200">

## On demand cloud computing for scientific research

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
- emulated web shell and desktop via [Apache _Guacamole](https://guacamole.incubator.apache.org/)  


+++

<img src="https://raw.githubusercontent.com/OpenDroneMap/OpenDroneMap/master/img/odm_image.png" height="150">

```shell
$ ezd -p
$ sudo usermod -aG docker $USER
$ exit
$ docker pull opendronemap/node-opendronemap:latest
$ docker run -d -p 3000:3000 opendronemap/node-opendronemap
Done!
```

@[1](install Docker and the Portainer.io - note the log output and the Portainer admin token)
@[2](change privileges to run Docker without `sudo`) 
@[3](exit and restart terminal window)
@[4](pull the latest version of Node OpenDroneMap)
@[5](Run the Container in `-d` detached mode on port `-p 3000:3000`)
@[7](Open the Node OpenDroneMap in a new browser tab on the VM IP on port :3000)

+++

## [Discovery Environment](https://de.cyverse.org)

<img src="assets/imagery/Discovery_white.png" height="200">

+++

<img src="assets/imagery/Discovery_white.png" height="200">

- Add your own Docker containers as "Tools"
- Build "Apps" with interfaces for users (equivalent command-line interface execution)
- Create a sequenced workflow by chaining one app to another in an automated workflow.
- Use application programming interfaces (APIs)

+++

### Visual Interactive Computing Environment (VICE)

<img src="assets/imagery/vice.png" width="400">

+++

<img src="assets/imagery/vice_diagram_small.png" width="800">

---

### Hosting and Publishing Data with CyVerse

---

### [DataCommons](http://datacommons.cyverse.org/)

<img src="assets/imagery/DataCommons_White.png" height="200">

- Easily share your data with your community members, and the public.
- "CyVerse Curated" data get a DOI
- "Community Released" data are living shared data
- Advantages over enterprise solutions

---

### Moving Data

- iRODS iCommands (CLI)
- WebDav (HTTPS)
- Discovery Environment 
- CyberDuck

---

### Want to learn more?

<img src="https://carpentries.org/images/TheCarpentries-opengraph.png" width="800">

https://carpentries.org

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

All digital images shown this presentation are available online and are the property of their creators, their web addresses are visible in the source code of this presentation at: https://github.com/cyverse-gis/uav-webinar/PITCHME.md 

---?image=assets/imagery/endslide.png


