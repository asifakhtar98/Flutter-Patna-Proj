# Flutter-Patna-Proj
<p align="center"> 
  <img src="readmeAssets/appName2x.png" alt="Pacman Logo"height="auto">
</p>
<h1 align="center"> Flutter Interview Project </h1>
<h3 align="center"> DEVELOPER DOCUMENTATION </h3>

<!--/////////////////////////////-->
<h3 align="center">Tools, Languages and Packages Used:</h3>
<p align="center"> <a href="https://developer.android.com" target="_blank" rel="noreferrer"> <img src="https://res.cloudinary.com/asifakhtarcloudinary/image/upload/v1641566862/AsifPortfolio/AndroidStudioLogo.png" alt="androidstudio" width="40" height="40"/> </a> <a href="https://developer.android.com" target="_blank" rel="noreferrer"> <img src="https://res.cloudinary.com/asifakhtarcloudinary/image/upload/v1641220897/AsifPortfolio/DartLang-480.png" alt="androidstudio" width="40" height="40"/> </a> <a href="https://appwrite.io" target="_blank" rel="noreferrer"> <img src="https://res.cloudinary.com/asifakhtarcloudinary/image/upload/v1641220978/AsifPortfolio/Flutter-480.png" alt="flutter" width="40" height="40"/> </a> <a href="https://www.arduino.cc/" target="_blank" rel="noreferrer">  </a><a href="https://appwrite.io" target="_blank" rel="noreferrer"> <img src="https://res.cloudinary.com/asifakhtarcloudinary/image/upload/v1641225517/AsifPortfolio/GetX1.png" alt="dart" width="40" height="40"/> </a> <a href="https://www.arduino.cc/" target="_blank" rel="noreferrer">  </a><a href="https://appwrite.io" target="_blank" rel="noreferrer"> <img src="https://res.cloudinary.com/asifakhtarcloudinary/image/upload/v1641220897/AsifPortfolio/DartLang-480.png" alt="dart" width="40" height="40"/> </a> <a href="https://www.arduino.cc/" target="_blank" rel="noreferrer">  </a> </p>

<!--////////////////////////////////////////////!-->
<p align="center"> 
  <img src="gif/pacman_game.gif" alt="Animated gif pacman game" height="282px" width="637">
</p>



![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<!-- ABOUT THE PROJECT -->
<h2 id="about-the-project"> :pencil: About The Project</h2>

<p align="justify"> 
  For those of you not familiar with Pacman, it's a game where Pacman (the yellow circle with a mouth in the above figure) moves around in a maze and tries to eat as many food pellets (the small white dots) as possible, while avoiding the ghosts (the other two agents with eyes in the above figure). If Pacman eats all the food in a maze, it wins.
</p>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<!-- OVERVIEW -->
<h2 id="overview"> :cloud: Overview</h2>

<p align="justify"> 
  In this project, the Pacman agent will find paths through his maze world, both to reach a particular location and to collect food efficiently. I implemented general search algorithms such as depth-first, breadth-first, uniform cost, and A* search algorithms which are used to solve navigation problems in the Pacman world.
</p>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<!-- PROJECT FILES DESCRIPTION -->
<h2 id="project-files-description"> :floppy_disk: Project Files Description</h2>

<ul>
  <li><b>search.py</b> - Where all of the search algorithms reside.</li>
  <li><b>searchAgents.py</b> - Where all of the search-based agents reside.</li>
  <li><b>pacman.py</b> - The main file that runs Pacman games. This file also describes a Pacman GameState types.</li>
  <li><b>game.py</b> - The logic behind how the Pacman world works.</li>
  <li><b>util.py</b> - Useful data structures for implementing search algorithms.</li>
</ul>

<h3>Some other supporting files</h3>
<ul>
  <li><b>graphicsDisplay.py</b> - Graphics for Pacman.</li>
  <li><b>graphicsUtils.py</b> - Support for Pacman graphics.</li>
  <li><b>textDisplay.py</b> - ASCII graphics for Pacman.</li>
  <li><b>ghostAgents.py</b> - Agents to control ghosts.</li>
  <li><b>keyboardAgents.py</b> - Keyboard interfaces to control Pacman.</li>
  <li><b>layout.py</b> - Code for reading layout files and storing their contents.</li>
  <li><b>autograder.py</b> - Project autograder.</li>
  <li><b>testParser.py</b> - Parses autograder test and solution files.</li>
  <li><b>testClasses.py</b> - General autograding test classes.</li>
  <li><b>test_cases/</b> - Directory containing the test cases for each scenario.</li>
  <li><b>searchTestClasses.py</b> - Project specific autograding test classes.</li>
</ul>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)


![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<!-- SCENARIO3 -->
<h2 id="scenario3"> :small_orange_diamond: Scenario 3: Finding the best path using Uniform Cost Search</h2>

<p>I have implemented the uniform-cost graph search (UCS) algorithm in the uniformCostSearch function in <code>search.py</code>.</p>
<p>While BFS will find a fewest-actions path to the goal, UCS will find paths that are “best” in other senses.</p>
<p>UCS agents differ only in the cost function they use.</p>
<p>The Pacman will quickly find a solution via running the following commands:</p>

<pre><code>$ python pacman.py -l mediumMaze -p SearchAgent -a fn=ucs</code></pre>
<pre><code>$ python pacman.py -l mediumDottedMaze -p StayEastSearchAgent</code></pre>
<pre><code>$ python pacman.py -l mediumScaryMaze -p StayWestSearchAgent</code></pre>

<p align="center"> 
<img src="gif/UCS.gif" alt="Animated gif UCS Algorithm" height="282px" width="637">
</p>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<!-- SCENARIO8 -->
<h2 id="scenario8"> :small_orange_diamond: Scenario 8: Suboptimal Search</h2>

<p>In this scenario, I have implemented a function that helps Pacman agent to find a path to the closest dot.</p>
<p>This function has been written in <code>searchAgents.py</code></p>
<p>The Pacman will quickly find a solution via running the following command:</p>

<pre><code>$ python pacman.py -l bigSearch -p ClosestDotSearchAgent -z .5</code></pre>

<p align="center"> 
<img src="gif/Suboptimal Search.gif" alt="Animated gif Suboptimal Search" height="282px" width="637">
</p>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<!-- CREDITS -->
<h2 align="center" id="credits"> :scroll: BY ASIF AKHTAR</h2>



Hi😎, I'm ASIF AKHTAR
=====================

![](https://media.giphy.com/media/Oz8UPcfxxvpSsNR7tB/giphy.gif)

### A passionate frontend developer from Assam India

![asifakhtar98](https://komarev.com/ghpvc/?username=asifakhtar98&label=Profile%20views&color=00bd97&style=flat-square)

[![asifakhtar98](https://github-profile-trophy.vercel.app/?username=asifakhtar98)](https://github.com/ryo-ma/github-profile-trophy)

[![](https://img.shields.io/twitter/follow/?logo=twitter&style=for-the-badge)](https://twitter.com/)

\- 🔭 I’m currently working on \*\*Freelance\*\* - 🌱 I’m currently learning \*\*Dart Advance, Flutter, Next JS\*\* - 👨‍💻 All of my projects are available at \[https://startupassamportfolio.web.app/\](https://startupassamportfolio.web.app/) - 📝 I regularly write articles on \[https://startupassamportfolio.web.app/\](https://startupassamportfolio.web.app/) - 📫 How to reach me \*\*asifakhtar91298.personal@gmail.com\*\* - 📄 Know about my experiences \[https://startupassamportfolio.web.app/\](https://startupassamportfolio.web.app/) - ⚡ Fun fact \*\*I do basically -> East Code Sleep Also Bath Twice A Day\*\*

### Connect with me:

[![asif-akhtar98](https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/stack-overflow.svg)](https://stackoverflow.com/users/asif-akhtar98) [![asifakhtar91298](https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg)](https://fb.com/asifakhtar91298) [![ios_android_developer_the_asif](https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg)](https://instagram.com/ios_android_developer_the_asif) [![asif-akhtar98](https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/hackerrank.svg)](https://www.hackerrank.com/asif-akhtar98)

![demo](https://user-images.githubusercontent.com/9840435/60266022-72a82400-98e7-11e9-9958-f9004c2f97e1.gif)

### Languages and Tools:

 [![android](https://raw.githubusercontent.com/devicons/devicon/master/icons/android/android-original-wordmark.svg)](https://developer.android.com) [ ![appwrite](https://www.vectorlogo.zone/logos/appwriteio/appwriteio-icon.svg) ](https://appwrite.io) [ ![arduino](https://cdn.worldvectorlogo.com/logos/arduino-1.svg) ](https://www.arduino.cc/) [ ![dart](https://www.vectorlogo.zone/logos/dartlang/dartlang-icon.svg) ](https://dart.dev) [ ![figma](https://www.vectorlogo.zone/logos/figma/figma-icon.svg) ](https://www.figma.com/) [ ![firebase](https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg) ](https://firebase.google.com/) [ ![flutter](https://www.vectorlogo.zone/logos/flutterio/flutterio-icon.svg) ](https://flutter.dev) [ ![gcp](https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg) ](https://cloud.google.com) [ ![git](https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg) ](https://git-scm.com/) [ ![ifttt](https://www.vectorlogo.zone/logos/ifttt/ifttt-ar21.svg) ](https://ifttt.com/) [ ![kubernetes](https://www.vectorlogo.zone/logos/kubernetes/kubernetes-icon.svg) ](https://kubernetes.io) [ ![mysql](https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg) ](https://www.mysql.com/) [ ![nodejs](https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg) ](https://nodejs.org) [ ![photoshop](https://raw.githubusercontent.com/devicons/devicon/master/icons/photoshop/photoshop-line.svg) ](https://www.photoshop.com/en) [ ![postman](https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg) ](https://postman.com) [ ![python](https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg) ](https://www.python.org) [ ![react](https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg) ](https://reactjs.org/) [ ![sketch](https://www.vectorlogo.zone/logos/sketchapp/sketchapp-icon.svg) ](https://www.sketch.com/) [![zapier](https://www.vectorlogo.zone/logos/zapier/zapier-icon.svg)](https://zapier.com) 

![asifakhtar98](https://github-readme-stats.vercel.app/api/top-langs?username=asifakhtar98&show_icons=true&theme=tokyonight&locale=en&layout=compact)

 ![asifakhtar98](https://github-readme-stats.vercel.app/api?username=asifakhtar98&show_icons=true&theme=tokyonight&locale=en)

![asifakhtar98](https://github-readme-streak-stats.herokuapp.com/?user=asifakhtar98&theme=highcontrast)
