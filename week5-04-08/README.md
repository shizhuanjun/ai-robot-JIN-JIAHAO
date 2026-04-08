AI机器人第6周作业<p>
效果图<p>
<img src=""><p>
操作过程：<p>
终端运行<p>
<pre><code>
cd ~/ros2_ws
colcon build --cmake-clean-cache
source ./install/setup.bash
ros2 run ros2_kitti_publishers kitti_publishers
</code></pre><p>
另一个终端运行<p>
<pre><code>
ros2 daemon start
rviz2
</code><pre>