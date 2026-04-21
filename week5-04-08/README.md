# AI机器人第五周作业
## 效果图
<img src="https://github.com/shizhuanjun/ai-robot-JIN-JIAHAO/blob/main/week5-04-08/img.png"><p>
<img src="https://github.com/shizhuanjun/ai-robot-JIN-JIAHAO/blob/main/week5-04-08/img1.png"><p>
## 操作过程：<p>
1.终端运行
<pre><code>cd ~/ros2_ws
colcon build --cmake-clean-cache
source ./install/setup.bash
ros2 run ros2_kitti_publishers kitti_publishers
</code></pre>
2.另一个终端运行
<pre><code>ros2 daemon start
rqt</code></pre>