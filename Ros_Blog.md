![Ros Picture](https://roboticsbiz.com/wp-content/uploads/2022/02/ros.jpg)

# Robot Operating System (ROS): Key to World of Robotics

## Table of Contents
<!-- UL -->
* Introduction
  * What is ROS ?
  * Significance of ROS in Robotics
  * History and Background of ROS
* Understanding ROS Fundamentals
  * Core Concepts and Architecture of ROS 
  * Key Components and their Roles
* Setting up the ROS Environment
  * Favourable Operating System for ROS 
  * Setting up a Workspace and Managing Packages
* Real-World Applications of ROS
* Conclusion
* References


## Introduction :
<p>Have you ever wondered how different components of a robot Communicate with one another? or how ROS helps a robot to Think, Sense and Act?. Lets find out answers to these questions. But before that let's take one step back that what ROS is and why do need it?<p>

![Ros Picture](https://hackaday.com/wp-content/uploads/2014/01/ros.png)

### What is ROS ?
ROS is __Robot Operating System__, although its not an actual operating system rather its an open source framework which provides a set of tools, applications, and software libraries that helps you build robot applications. One of the major strengths of ROS is its vast community and its open-source nature which helps many developers around the world to contribute to ROS by creating and sharing packages (pre-built functionalities) that you can readily use to expand your robot's capabilities. This collaborative ecosystem accelerates progress and democratizes robotics, making advanced technologies accessible to enthusiasts, researchers, and industries alike.

### Significance of ROS in Robotics :
<p>Basically the significance of ROS in robotics is that it provides a special toolbox that helps people create robots with less effort and with more creativity. Let's talk about some of its features which makes ROS essential for Robotics:<p>

* __Building Robots with Ease__ : Due to its open source nature, ROS allows developers to reuse code contributed by developers all around the world, which not only saves time but also makes it simpler to construct new robots.

* __Testing in Virtual world__ : Before constructing a real robot, you can test it in a computer-simulated world (such as Gazebo) with ROS, which not only saves time but also helps to avoid unintended consequences.

![Ros Picture](https://opencloudware.com/wp-content/uploads/2021/03/robot-operating-system-ros-intro.png)

* __Helpful Robotics Community__ : A huge community of people who use ROS,  share their skills and resources for constructing robots. Learning and problem-solving are made simpler by this welcoming community.

* __Real-Life Applications__ : Robots aren't just for labs, they have applications outside of laboratories as well. Companies utilize ROS to build robots for a variety of tasks, including space exploration, hospital care, and factory work.  

<p>In a nutshell, ROS is like a magic toolbox that improves teamwork, makes robots smarter, and makes robot-building more approachable for anyone. It is influencing robotics' direction and creating a more interesting, robotic world!<p>

### History and Background of ROS :
Roboticists are now highly fond of the ROS (__Robot Operating System__). It is being used, promoted, and supported by researchers, enthusiasts, and even robotics firms. It wasn't always this way, though. Early on, ROS was a little-known program that was only used by a few robotics nerds. How did ROS become the robotics standard it is today? Let's look at how ROS reached its present position of superiority.

![ROS Picture](https://www.theconstructsim.com/wp-content/uploads/2019/07/A-History-of-ROS-Robot-Operating-System.png)

Earlier Ros was started as a personal project of __Keenan Wyrobek__ (also the co-founder and head of product and Engineering at __Zipline__) and __Eric Berger__ while at Stanford, as an attempt to remove the problem of __reinventing the wheel__ situation from which robotics was suffering, meaning spending time and effort to recreate something which already exists in the ROS community. It's about avoiding unnecessary duplication of work and using existing tools and packages to build robots more efficiently. 

In order to address that issue, Eric and Keenan established the __Stanford Personal Robotics Program__ in 2006. Its goal was to provide a framework that would enable processes to communicate with one another as well as some tools to build code on top of that framework. The Personal Robot, which they would also develop, was intended to serve as a testbed and an example for others, and all that framework was to be used to write programming for it.

![ROS Picture](https://th.bing.com/th/id/R.6470cc7475c85dc7e26f994d1d698fe0?rik=etKfhtFRAzqBDw&riu=http%3a%2f%2fwww.robotsvoice.com%2fwp-content%2fuploads%2f2016%2f09%2fPR2-1900x1520_c.jpg&ehk=BqPhZVWCghadhyGXYcwJW7IqVXUBVAN5%2fzRUG%2fDxukY%3d&risl=&pid=ImgRaw&r=0)

At some point around 2008, Keenan and Eric met with __Scott Hassan__, investor and the founder of __Willow Garage__, a research center with a focus on robotics products. Scott found their idea so interesting that he decided to fund it and start a __Personal Robotics Program__ inside Willow Garage with them. The Robot Operating System was born and the __PR2 robot__ with it. Actually, the ROS project became so important that all the other projects of Willow Garage were discarded and Willow Garage concentrated only on the development and spread of ROS.

As a result first version of ROS was officially released in 2010 known as __ROS 1.0__ or __ROS Electric Turtle__. Since then, ROS has grown into a robust and influential platform that has transformed the world of robotics, enabling developers to create innovative and sophisticated robotic systems with ease, and its not over yet ROS keeps growing and improving. Its newest version __ROS 2.0__ aims to address the limitations of __ROS 1.0__ and is also designed to make robots even smarter and safer.

## Understanding ROS Fundamentals :
To understand the basics of ROS it is divided into three levels of concepts: the __Filesystem level__, the __Computation Graph level__, and the __Community level__. Lets understand these concepts and levels one by one.

### Core Concepts and Architecture of ROS :
* __ROS Filesystem Levels__ : The filesystem level concepts mainly cover ROS resources that are available on disk as you install ROS on your system, such as Packages, Metapackages, Package Manifests, Message(msg) types, Service(srv) types. 

* __ROS Computation Graph Level__ : The Computation Graph is the peer-to-peer network of ROS processes that are processing data together. The basic Computation Graph concepts of ROS are nodes, Master, Parameter Server, messages, services, topics, and bags, all of which provide data to the Graph in different ways.

![ROS Picture](https://static.packt-cdn.com/products/9781838649326/graphics/assets/f6015922-13c2-4bfb-aa73-ebdd063cb561.png)

<p>The ROS Master acts as a nameservice in the ROS Computation Graph. It stores topics and services registration information for ROS nodes.<p>

* __ROS Community Level__ : The ROS Community level concepts are ROS resources that enable separate communities to exchange software and knowledge, also help the communities to resolve issues that are faced by other communities. These resources include Repositories, Distributions, the most famous one ROS wiki and many more.

To understand the above concepts in more detail you can visit [ROS wiki](http://wiki.ros.org/ROS/Concepts). 
### Key Concepts and their Role :
Now lets understand some key concepts of ROS which play a crucial role while building a robotic application, lets discuss them :

* __Nodes__ : Nodes are the building blocks of ROS, these are individual units of computation which are responsible for specific tasks. For example, one node controls a laser range-finder, one node controls the wheel motors, one node performs localization, and so on. These nodes communicate with each other by sending and receiving messages.  

* __Messages__ : Messages are the data formats through which nodes communicate with each other. They define the structure and content of information exchanged between nodes. ROS supports a variety of message types, from simple data types like integers and strings to more complex structures like custom messages for robot poses or sensor readings.

* __Topics__ : Topics facilitate communication between nodes by sending messages through a transport system with publish / subscribe semantics. Topics enable one-to-many communication, allowing multiple nodes to share information efficiently. For example, a camera node may publish image data on a "camera_feed" topic, while multiple other nodes (e.g., object detection, navigation) can subscribe to this topic to process the images.

![ROS Picture](https://miro.medium.com/max/1400/1*fyWZBFPKEoLedhvo7nZyMQ.jpeg)

* __Services__ : Services enable one-to-one communication between nodes. Unlike topics that facilitate ongoing communication, services follow a request-response pattern. A node can request a particular service from another node, which then provides a response. This mechanism is ideal for tasks that require interaction with nodes on an as-needed basis.

* __Actions__ : Actions are similar to services but are designed for tasks that take a longer time to complete, such as moving a robot to a specific location or executing a complex operation. Actions support asynchronous behavior and provide feedback on the progress of the task.

<p>These key components of ROS create a powerful communication infrastructure that allows developers to build complex and intelligent robotic systems that can perform exceptionally high level task.<p>

## Setting up the ROS Environment
<p>Before we move on to build robots using ROS, its important to first install necessary software and libraries on your System. Once installed, you'll have access to powerful tools and a robust ecosystem for developing and experimenting with robots in the exciting world of ROS. <p>

### Favourable Operating System for ROS
When it comes to selecting the best operating system for working with ROS, __Linux__ stands out as the best option. Linux is the recommended platform for seamless integration and development of ROS because Linux was the primary platform for its design and optimization. One of the key advantages of Linux that neither __Mac__ nor __Windows__ have is its performance and stability, which makes it an excellent choice for resource-intensive applications such as robotic simulations and real-time control. However, work on the Windows and Mac OS versions of ROS is still ongoing. To make ROS function on Windows, there are a few workarounds.

### Setting up Workspace/Package Management
<p>Before we start making the main part of the building lets starts by making base of it that in this case before we start making the robot we have to define the workspace for it. So lets see step by step procedure for that.

* After you have successfully installed ROS on your system, open a terminal and create a workspace (or working directory) and a sub-folder named 'Ros_ws' and 'src' through linux commands. Then navigate to your 'Ros_ws' directory and perform catkin_make (method used to organize and build your ROS code).

> mkdir  -p  ~/Ros_ws/src                                         
> cd  ~/Ros_ws/  
> catkin_make

* Now navigate to 'src' folder of your workspace and create a package using 'catkin_create_pkg' command named my_robot with suitable dependencies.

> catkin_create_pkg  my_robot  rospy  std_msgs

* After that navigate back to the root of your workspace and perform catkin_make to build your workspace. If you want that ROS finds your package easily then source your worspace as:
> source/devel/setup.bash

So in this way you can make additional packages by repeating the steps and also you can organize them by creating sub-directories in the 'src' folder for different projects or functionalities. For more information you can see [tutorial-1](http://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment) of ROS_wiki.org.<p>

## Real-World Applications of ROS
<p>ROS has found its way into numerous real-world projects and applications across various industries, showcasing its versatility and impact on modern robotics. Lets see these awesome ROS applications.<p>

* __Healthcare Assistants__ : ROS-enabled robots are revolutionizing healthcare by helping doctors with duties like drug delivery, patient monitoring, and cleaning. Particularly when it comes to contagious diseases, these robots increase productivity while minimizing human interaction.

* __Autonomous Vehicles__ : A key technology in the creation of autonomous vehicles is ROS. It offers the technological foundation for perception, management, and navigation, enabling vehicles to move through and communicate with one another safely in challenging settings.

![ROS Picture](https://qtxasset.com/styles/breakpoint_xl_880px_w/s3/sensorsmag/1557156950/HERO.jpg?mFGa53Yqlxk9bvrpWrR4c.DCNcwqHF1.&itok=NpvWCRlz)

For example the NVIDIA's __Autonomous Research Vehicle__ (ARV) which is a self-driving car platform that utilizes ROS for its software infrastructure. The ARV is equipped with advanced sensors and NVIDIA's AI technology to enable autonomous navigation and perception.

* __Space Exploration__ : ROS is also used in the development of robotic systems for space exploration. It aids in the control and operation of robotic arms on spacecraft, rovers on planetary surfaces, and even satellites. For example __Robonaut2__ (R2) humanoid Robot. In 2012 NASA switched R2's software over to ROS and used Gazebo (Simulation platform for robots), Open Robotics’ 3D robotics simulator, to build a model of the robot and the __International Space Station__ (ISS). By 2014, R2, and its ROS-based software, was up and running on the ISS. This was the first confirmed use of ROS in space.(For more info you can also check the Nasa's official website).

* __Service Robot__ : ROS-powered service robots are employed in settings like hotels, airports, and shopping malls, providing information, delivering items, and enhancing customer service experiences. Service Robots have also impacted various industries by automating tasks, enhancing efficiency, and improving overall operations. Take example of fetch robotics that used __Autonomous mobile robots__ (AMRs) to optimize distribution operations because they are

![ROS Picture](https://fetch3.wpenginepowered.com/wp-content/uploads/2021/01/Fetch-Robotics-PalletTransport1500-Docking.jpg)

 incredibly flexible, scalable, and can integrate into other forms of fixed automation such as conveyor, ASRSs, sortation systems as well.

<p>There are multiple other implementations of ROS in other areas; these real-world projects and applications showcase ROS's impact on diverse industries, highlighting its role in defining the future of robotics and automation. ROS continues to spur innovation and change how we engage with robots in various facets of our life, from healthcare to outer space..<p>

## Conclusion
To understand the above concept properly, lets see one project based on ROS. In this we have created a simulation environment in __Gazebo__ (simulation platform) to spawn a differential drive robot using ROS. Also displaying Hello World mesaage on the terminal as soon as the World is launched.

![Gazebo World](https://user-images.githubusercontent.com/97186785/167906069-6745a759-416f-4ffc-9db4-d8812ad23caf.png)

<p>Lets understand the procedure step by step : <p>

* First we have to make a working directory or a workspace, like in this case it is my_robot along with a source folder (src) inside it will create a package named Build_MyWorld. 

* Then will create a folder name world inside the package we created. In this folder will create a urdf file (Giving description about the world) of the world. 

* Then will create a script folder in which will write a code so that whenever the world is launched it shows "Hello World" in the terminal.

That's how will make each and every robotics related project like this. But to start in a proper way for beginners you must follow [Ros Wiki](http://wiki.ros.org/ROS/Tutorials) tutorials to master ROS.


## References for the above Material

* [Picture-1](https://roboticsbiz.com/wp-content/uploads/2022/02/ros.jpg)
* [Picture-2](https://hackaday.com/wp-content/uploads/2014/01/ros.png)
* [Picture-3](https://opencloudware.com/wp-content/uploads/2021/03/robot-operating-system-ros-intro.png)
* [Picture-4](https://www.theconstructsim.com/wp-content/uploads/2019/07/A-History-of-ROS-Robot-Operating-System.png)
* [Picture-5](https://th.bing.com/th/id/R.6470cc7475c85dc7e26f994d1d698fe0?rik=etKfhtFRAzqBDw&riu=http%3a%2f%2fwww.robotsvoice.com%2fwp-content%2fuploads%2f2016%2f09%2fPR2-1900x1520_c.jpg&ehk=BqPhZVWCghadhyGXYcwJW7IqVXUBVAN5%2fzRUG%2fDxukY%3d&risl=&pid=ImgRaw&r=0)
* [Picture-6](https://static.packt-cdn.com/products/9781838649326/graphics/assets/f6015922-13c2-4bfb-aa73-ebdd063cb561.png)
* [Picture-7](https://miro.medium.com/max/1400/1*fyWZBFPKEoLedhvo7nZyMQ.jpeg)
* [Picture-8](https://qtxasset.com/styles/breakpoint_xl_880px_w/s3/sensorsmag/1557156950/HERO.jpg?mFGa53Yqlxk9bvrpWrR4c.DCNcwqHF1.&itok=NpvWCRlz)
* [Picture-9](https://fetch3.wpenginepowered.com/wp-content/uploads/2021/01/Fetch-Robotics-PalletTransport1500-Docking.jpg)
* [Picture-10](https://user-images.githubusercontent.com/97186785/167906069-6745a759-416f-4ffc-9db4-d8812ad23caf.png)

for the contents, I have used the following websites :

* [The construct](https://www.theconstructsim.com/history-ros/)
* [Ros wiki](http://wiki.ros.org/ROS/Tutorials)
* [The Robot Report](https://www.therobotreport.com/open-robotics-developing-space-ros/#:~:text=Its%20use%20began%20at%20ROSCon,International%20Space%20Station%20(ISS).)
* [Fetch Robotics](https://fetchrobotics.com/distribution/)
* [Nividia](https://www.nvidia.com/en-in/self-driving-cars/)

Also i took some help from open AI or Chatgpt 