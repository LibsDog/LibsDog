<h1 align="center">课题组学习入门指南</h1>

<p align="center"> </p>


> Embodied AI（具身智能）入门的路径以及高质量信息的总结, 期望是按照路线走完后, 新手可以快速建立关于这个领域的认知, 希望能帮助到各位入门具身智能的朋友, 欢迎点Star、分享与提PR🌟~<br>【 <a href="https://github.com/tianxingchen/Embodied-AI-Guide">Embodied-AI-Guide</a>, Latest Update: May. 1, 2025 】<img alt="GitHub repo stars" src="https://img.shields.io/github/stars/TianxingChen/Embodied-AI-Guide"> ![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2FTianxingChen%2FEmbodied-AI-Guide&label=Daily%20Visitors&labelColor=%232ccce4&countColor=%23d9e3f0)


# Lumina具身智能社区: [点击访问](https://lumina-embodied.ai)

> Embodied-AI-Guide项目很快将会以网页版wiki的形式上传到Lumina具身智能社区网站，敬请期待。如果你对合作构建Lumina具身社区感兴趣（目前更倾向于机构、社区间合作），欢迎邮件联系<a href="mailto:lumina.embodiedai@gmail.com">lumina.embodiedai@gmail.com</a>或联创微信<code>TianxingChen_2002</code>（请备注机构+姓名与来意）

**扫描右下图进入`Embodied-AI-Guide@Lumina社区`交流群**:

<table>
  <tr>
    <td>
      <img src="./files/images/logo.png" alt="Task Descriptions">
    </td>
    <td>
      <img src="./files/QR-Code.png" alt="Task Descriptions">
    </td>
  </tr>
</table>


# Contents - 目录

<nav>
  <ul>
    <li><a href="#start">1. Start From Here - 从这里开始</a></li>
    <li><a href="#info">2. Useful Info - 有利于搭建认知的资料</a></li>
    <li><a href="#algorithm">3. Algorithm - 算法</a>
      <ul>
        <li><a href="#common-tools">3.1 Common Tools - 常用工具</a></li>
        <li><a href="#foundation-models">3.2 Foundation Models - 基础模型</a></li>
        <li><a href="#robot-learning">3.3 Robot Learning - 机器人学习</a>
          <ul>
            <li><a href="#robot_autonomy">3.3.1 ETH & TTIC & UdeM Robot Autonomy - 自主机器人</a></li>
            <li><a href="#mpc">3.3.2 Model Predictive Control - 模型预测控制</a></li>
            <li><a href="#rl">3.3.3 Reinforcement Learning - 强化学习</a></li>
            <li><a href="#il">3.3.4 Imitation Learning - 仿人学习</a></li>
            <li><a href="#mila_robot_learning">3.3.5 MILA & UdeM Robot Learning - 机器人学习课程</a></li>
          </ul>
        </li>
        <li><a href="#llm_robot">3.4 LLM for Robotics - 大语言模型在机器人学中的应用</a></li>
        <li><a href="#vla">3.5 Vision-Language-Action Models - VLA模型</li>
        <li><a href="#cv">3.6 Computer Vision - 计算机视觉</a>
          <ul>
            <li><a href="#2dv">3.6.1 2D Vision - 二维视觉</a></li>
            <li><a href="#3dv">3.6.2 3D Vision - 三维视觉</a></li>
            <li><a href="#4dv">3.6.3 4D Vision - 四维视觉</a></li>
            <li><a href="#vp">3.6.4 Visual Prompting - 视觉提示</a></li>
            <li><a href="#ag">3.6.5 Affordance Grounding - 可供性锚定</a></li>
          </ul>
        </li>
        <li><a href="#cg">3.7 Computer Graphics - 计算机图形学</a></li>  
        <li><a href="#mm">3.8 Multimodal Models - 多模态模型</a></li>  
        <li><a href="#navigation">3.9 Robot Navigation - 机器人巡航</a></li>  
        <li><a href="#embodied-ai-4-x">3.10 Embodied AI for X - 具身智能+X</a>
          <ul>
            <li><a href="#medical">3.10.1 EAI for Healthcare - 具身医疗</a></li>
            <li><a href="#uav">3.10.2 UAV - 无人机</a></li>
            <li><a href="#ad">3.10.3 Autonomous Driving - 自动驾驶</a></li>
          </ul>
        </li>
      </ul>
    </li>
    <li><a href="#control">4 Control and Robotics - 控制论与机器人学基础</a>
      <ul>
        <li><a href="#41-控制理论基础">4.1 控制理论基础</li>
        <ul>
          <li><a href="#411-经典控制原理">4.1.1 经典控制原理</li>
          <li><a href="#412-现代控制理论线性系统控制">4.1.2 现代控制理论(线性系统控制)</li>
          <li><a href="#413-先进控制技术">4.1.3 先进控制技术</li>
        </ul>
        <li><a href="#42-机器人学导论">4.2 机器人学导论</li>
        <ul>
          <li><a href="#421-推荐材料">4.2.1 推荐资料</li>
          <li><a href="#422-机器人运动学-kinematics-与动力学-dynamics">4.2.2 机器人运动学与动力学</li>
          <li><a href="#423-里程计和同步定位与建图-odometryslam">4.2.3 里程计和同步定位与建图 (Odometry&SLAM)</li>
          <li><a href="#424-杂项-misc">4.2.4 杂项</li>
        </ul>
      </ul>
    </li> 
    <li><a href="#hardware">5. Hardware - 硬件</a>
      <ul>
        <li><a href="#embedded">5.1 Embedded - 嵌入式</a></li>
        <li><a href="#mechanical">5.2 Mechanical Design - 机械设计</a></li>
        <li><a href="#robosystem">5.3 Robot System Design - 机器人系统设计</a></li>
        <li><a href="#sensors">5.4 Sensors - 传感器</a></li>
        <li><a href="#tactile">5.5 Tactile Sensing - 触觉感知</a></li>
        <li><a href="#companies">5.6 Companies - 公司</a></li>
      </ul>
    </li>
    <li><a href="#software">6. Software - 软件</a>
      <ul>
