1.ubnutu安装ROS2<br>
<pre><code>wget http://fishros.com/install -O fishros && bash fishros;</code></pre>
2.验证安装<br><br>
&ensp;(1)打开终端<br>
<pre><code>ros2 run turtlesim turtlesim_node</code></pre>
&ensp;(2)新开一个终端运行 
<pre><code>ros2 run turtlesim turtle_teleop_key</code></pre>
3.安装openclaw<br>
<pre><code>curl -fsSL https://openclaw.ai/install.sh | bash</code></pre>
&ensp;启动小龙虾<br>
<pre><code>openclaw gateway</code></pre>
