# AI机器人第十二周作业
## 手机摄像头、ArUco 识别
### 效果图
<img src="img/img.jpg" width="300"><p>
### 操作步骤
1.在WSL和手机中安装Tailscale
<pre><code>curl -fsSL https://tailscale.com/install.sh | sh
sudo service tailscaled start
sudo tailscale up
</code></pre>
 执行<code>sudo tailscale up</code>后，按照终端提示登录自己的账号<p>
 这里登录的账号应当与手机端保持一致。<p>
 查看当前网络状态：
 <code><pre>tailscale status
tailscale ip -4
</code></pre>
2.给WSL加上 SSH 登录学习测试
 <pre><code>sudo apt update
 sudo apt install openssh-server -y
 sudo service ssh start
 </code></pre>
2.1确认SSH服务启动
<pre>sudo service ssh status</pre>
然后查看Tailscale在WSL中的地址
<pre>tailscale ip -4</pre>
3.安装python库
<pre><code>sudo apt update
sudo apt install python3-pip -y
pip3 install -r week12_starters/requirements.txt
</code></pre>
这一步完成后，再运行桥接程序。<p>
如果直接运行程序时看到下面这类报错：<p>
<pre>No module named 'flask'</pre>
通常就说明依赖还没有安装完成。<p>
4.运行相机接收脚本
<pre><code>python3 week12_starters/camera_bridge.py</code></pre>
5.用手机浏览器访问页面
在手机浏览器中打开：<p>
<pre>https://100.109.19.11:5000</pre>
    