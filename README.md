
<h1 align="center">ROS Essentials</h1>

## ROS Commands
<ul>
  <li><code>roscore</code> - to run the main ros server</li>
  <li><code>roscd</code> - to switch to main ros directory</li>
  <li><code>roscd [ros_package_name] [ros_node_name]</code> - to switch to the specific package inside the ros directory</li>
</ul>


## Creating a ROS package
Here, the packages are created within the <i>src</i> sub-directory of the <i>catkin_ws</i> directory
<pre><code>catkin_create_pkg [package-name] [dependency-1] [dependency-2] [dependency-3]</code></pre>
Make sure to run <code>catkin_make</code> to create and compile the package
