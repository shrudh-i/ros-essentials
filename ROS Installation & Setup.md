# Installation of ROS
<p>Here, I'm installing ROS Noetic which is available for Ubuntu 20.04. With reference to the ROS documentation: http://wiki.ros.org/noetic/Installation/Ubuntu.</p>

<p>Open a terminal in the home directory and proceed to install by following the below steps!</p>
<hr>

## 1 Setup your sources.list - Mirrors
<p>Mainly used to ensure Ubuntu accepts the ROS packages</p>
<pre><code>sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'</code></pre>

## 2 Setting up the keys 
<p>If you haven't installed curl yet, run: <code>sudo apt-get install curl</code> and then proceed to execute this command:</p>
<pre><code>curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -</code></pre>

## 3 Installation
<p>Run <code>sudo apt update</code> to make sure all Debian packages are upto date.</p>
<p>For the ROS installation, I've gone with a <b>Desktop-Full Install</b> by executing:</p>
<pre><code>sudo apt install ros-noetic-desktop-full</code></pre>

## 4 Environment Setup 
<p>Instead of sourcing ROS everytime a new terminal is opened, it can be automated by adding the source command in the bash file</p>
<pre><code>echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
<br>source ~/.bashrc</code></pre>

<p align="center">
  <img width="569.3240901213" height="450" src="https://user-images.githubusercontent.com/89002422/136798855-1799b50f-a87c-4b87-a029-b13a85c6beb6.png">
</p>

## 5 Create: Catkin Workspace
<p>
  The catkin workspace is a directory where existing catkin packages can be created/modified
  <br>To build the catkin workspace:
</p>
<pre><code>mkdir -p ~/catkin_ws/src
<br>cd ~/catkin_ws/
<br>catkin_make</code></pre>
<p>Here, running <code>catkin_make</code> for the first time, creates a <code>CMakeLists.txt</code> link in the src directory. Along with that, three sub-directories:</p>


## 6 Clone: ROS Noetic Distrubution GitHub Repo
## 7 Test Installation w/ C++ Nodes
## 8 Test & Fix Installation w/ Python Nodes
