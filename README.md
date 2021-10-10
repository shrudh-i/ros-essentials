# ROS Essentials
Starting off from an absolute beginner level to advanced levels
<hr>

## A. Installation of ROS
<p>Here, I'm installing ROS Noetic which is available for Ubuntu 20.04. With reference to the ROS documentation: http://wiki.ros.org/noetic/Installation/Ubuntu.</p>

<p>Open a terminal in the home directory and proceed to install by following the below steps!</p>

### A.1 Setup your sources.list - Mirrors
<p>Mainly used to ensure Ubuntu accepts the ROS packages</p>
<pre><code>sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'</code></pre>

### A.2 Setting up the keys 
<p>If you haven't installed curl yet, run: <code>sudo apt-get install curl</code> and then proceed to execute this command:</p>
<pre><code>curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -</code></pre>

### A.3 Installtion
<p>Run <code>sudo apt update</code> to make sure all Debian packages are upto date.</p>
<p>For the ROS installation, I've gone with a <b>Desktop-Full Install</b> by executing:</p>
<pre><code>sudo apt install ros-noetic-desktop-full</code></pre>

### A.4 Environment Setup 
<p>Instead of sourcing ROS everytime a new terminal is opened, it can be automated by adding the source command in the bash file</p>
<pre><code>echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
<br>source ~/.bashrc</code></pre>
