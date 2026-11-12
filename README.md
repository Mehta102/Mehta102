<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=header&text=Om%20Mehta&fontSize=58&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=AI%20and%20Robotics%20Software&descSize=20&descAlignY=60" alt="Om Mehta" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=18&pause=1200&color=36BCF7&center=true&vCenter=true&width=560&lines=BSc+Computer+Science+with+AI%2C+First+Class;Machine+learning+%C2%B7+computer+vision+%C2%B7+ROS2;Moving+forward+in+depth+with+robotics" alt="Typing tagline" />
</p>

<p align="center">
  <a href="https://linkedin.com/in/ommehta5"><img src="https://img.shields.io/badge/LinkedIn-ommehta5-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:ommehta102@gmail.com"><img src="https://img.shields.io/badge/Email-get%20in%20touch-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

---

### 👋 About

I graduated with a First in Computer Science with AI, and the part I keep coming back to is making software that has to *react* to something. A robot that has to get round a chair it did not know was there. A model that watches a game screen and has to decide whether what just happened is worth talking about.

I learn fastest by building the thing and watching it fail, so most of what is below started as a "can I actually make this work?" and ended up teaching me more than the lectures did.

```bash
$ ros2 node list
/om_mehta

$ ros2 topic echo /status
data: "open to graduate AI, ML and robotics roles"
---
```

### 🔧 Things I've built

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>🎮 <a href="https://github.com/Mehta102/backseater-ai">Backseater AI</a></h4>
      My final year project. It watches a game as you play, works out what just happened on screen, and talks to you about it like a mate sitting behind you on the sofa. The hard part was not getting it to talk, it was getting it to <i>shut up</i> at the right moments.<br><br>
      <sub><b>Built with:</b> Python · OpenCV · Tesseract · scikit-learn · text to speech</sub>
    </td>
    <td width="50%" valign="top">
      <h4>🤖 Autonomous ROS2 Robot</h4>
      A simulated robot in Gazebo that drives itself around a room with no map. Three behaviours stacked by priority: dodge what is in front of it, follow a wall if there is one, otherwise just wander and see what it finds.<br><br>
      <sub><b>Built with:</b> ROS2 · Gazebo · Python · LIDAR</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4>🪑 <a href="https://github.com/Mehta102/DeskMateAI">Deskmate AI</a></h4>
      Point it at a room and it tells you whether your furniture is in a sensible place, then suggests a better layout. Part computer vision, part "what would an interior designer say".<br><br>
      <sub><b>Built with:</b> Python · deep learning · Flutter · React · Unity</sub>
    </td>
    <td width="50%" valign="top">
      <h4>🌡️ IoT Monitor</h4>
      A small ESP32 build that reads temperature and humidity and sets a buzzer off when things get too hot. Small, but it was my first time chasing a bug that turned out to be a wiring problem and not a code one.<br><br>
      <sub><b>Built with:</b> C++ · ESP32 · sensors · Wokwi</sub>
    </td>
  </tr>
</table>

### 🧠 How the robot decides

Roughly how the ROS2 robot picks what to do each tick (simplified from the real thing):

```python
def decide(scan):
    if scan.front < 0.5:        # something is right in front of me
        return turn_away()
    if scan.side < 1.0:         # a wall is nearby, hug it
        return follow_wall()
    return wander()             # nothing to react to, explore
```

The order matters more than the code. Safety first, then the clever stuff.

### 🧰 Tech I use

**Languages**<br>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++">
<img src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white" alt="C#">
<img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white" alt="Dart">
<img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin">
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript">

**AI and robotics**<br>
<img src="https://img.shields.io/badge/ROS2-22314E?style=flat-square&logo=ros&logoColor=white" alt="ROS2">
<img src="https://img.shields.io/badge/Gazebo-FF6F00?style=flat-square" alt="Gazebo">
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn">
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" alt="OpenCV">
<img src="https://img.shields.io/badge/Reinforcement%20learning-2c5364?style=flat-square" alt="Reinforcement learning">

**Tools**<br>
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git">
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux">
<img src="https://img.shields.io/badge/Unity-000000?style=flat-square&logo=unity&logoColor=white" alt="Unity">
<img src="https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white" alt="Figma">

### 🌱 Right now

- Going deeper into robotics: navigation, SLAM and control, building on the ROS2 simulation work
- Working back through data structures and algorithms until they are second nature
- Tidying up my older projects so they are actually readable by someone who is not me

> Moving forward in depth with robotics, one simulated crash at a time.

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer" alt="" />
</p>
