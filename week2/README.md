# AI机器人第二周作业
## 效果图<p>
<img src="https://github.com/shizhuanjun/ai-robot-JIN-JIAHAO/blob/main/week2/week2.png"><p>
## 操作步骤<p>
1.让小乌龟前进<br>
<pre><code>ros2 topic pub /turtle1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 1.0, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 0.0}}"</code></pre>
2.监听小乌龟位置<br>
<pre><code>ros2 topic echo /turtle1/pose</code></pre>