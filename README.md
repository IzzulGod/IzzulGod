<svg viewBox="0 0 800 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Gradients -->
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d1117;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#161b22;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#21262d;stop-opacity:1" />
    </linearGradient>
    
    <linearGradient id="textGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#58a6ff;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#79c0ff;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#a5f3fc;stop-opacity:1" />
    </linearGradient>
    
    <linearGradient id="accentGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#f78166;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#ff7b72;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#ffa657;stop-opacity:1" />
    </linearGradient>
    
    <!-- Glow effect -->
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge> 
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    
    <!-- Code animation -->
    <style>
      .code-float { animation: float 3s ease-in-out infinite; }
      .code-float-delay { animation: float 4s ease-in-out infinite 1s; }
      .code-float-delay2 { animation: float 3.5s ease-in-out infinite 2s; }
      .terminal-cursor { animation: blink 1s infinite; }
      .circuit-line { animation: pulse 2s ease-in-out infinite; }
      
      @keyframes float {
        0%, 100% { transform: translateY(0px); opacity: 0.7; }
        50% { transform: translateY(-10px); opacity: 1; }
      }
      
      @keyframes blink {
        0%, 50% { opacity: 1; }
        51%, 100% { opacity: 0; }
      }
      
      @keyframes pulse {
        0%, 100% { opacity: 0.3; }
        50% { opacity: 0.8; }
      }
    </style>
  </defs>
  
  <!-- Background -->
  <rect width="800" height="300" fill="url(#bgGrad)" rx="15"/>
  
  <!-- Circuit pattern background -->
  <g opacity="0.1">
    <path d="M50 50 L150 50 L150 100 L250 100" stroke="#58a6ff" stroke-width="1" fill="none" class="circuit-line"/>
    <path d="M750 250 L650 250 L650 200 L550 200" stroke="#58a6ff" stroke-width="1" fill="none" class="circuit-line"/>
    <circle cx="150" cy="50" r="3" fill="#58a6ff"/>
    <circle cx="150" cy="100" r="3" fill="#58a6ff"/>
    <circle cx="650" cy="250" r="3" fill="#58a6ff"/>
    <circle cx="650" cy="200" r="3" fill="#58a6ff"/>
  </g>
  
  <!-- Floating code elements -->
  <g class="code-float" opacity="0.6">
    <text x="70" y="80" font-family="'Courier New', monospace" font-size="14" fill="#79c0ff">def hello():</text>
    <text x="85" y="100" font-family="'Courier New', monospace" font-size="12" fill="#a5f3fc">print("AI")</text>
  </g>
  
  <g class="code-float-delay" opacity="0.5">
    <text x="650" y="60" font-family="'Courier New', monospace" font-size="12" fill="#ffa657">&lt;Robot/&gt;</text>
    <text x="630" y="80" font-family="'Courier New', monospace" font-size="10" fill="#ff7b72">while(true)</text>
  </g>
  
  <g class="code-float-delay2" opacity="0.4">
    <text x="80" y="220" font-family="'Courier New', monospace" font-size="11" fill="#79c0ff">import torch</text>
    <text x="650" y="230" font-family="'Courier New', monospace" font-size="11" fill="#a5f3fc">ros2 run</text>
  </g>
  
  <!-- Programming symbols scattered -->
  <text x="200" y="40" font-family="'Courier New', monospace" font-size="16" fill="#58a6ff" opacity="0.3">{}</text>
  <text x="550" y="45" font-family="'Courier New', monospace" font-size="18" fill="#f78166" opacity="0.4">[]</text>
  <text x="150" y="250" font-family="'Courier New', monospace" font-size="20" fill="#79c0ff" opacity="0.3">()</text>
  <text x="600" y="280" font-family="'Courier New', monospace" font-size="14" fill="#ffa657" opacity="0.4">;</text>
  
  <!-- Main title -->
  <g transform="translate(400, 120)">
    <!-- Hi! -->
    <text x="-180" y="0" font-family="'Arial Black', sans-serif" font-size="32" font-weight="bold" fill="url(#textGrad)" filter="url(#glow)">Hi!</text>
    
    <!-- I'm -->
    <text x="-120" y="0" font-family="'Arial', sans-serif" font-size="28" fill="#e6edf3">I'm</text>
    
    <!-- IzzulGod with special styling -->
    <text x="-55" y="0" font-family="'Arial Black', sans-serif" font-size="36" font-weight="bold" fill="url(#accentGrad)" filter="url(#glow)">IzzulGod</text>
  </g>
  
  <!-- Subtitle -->
  <text x="400" y="170" font-family="'Arial', sans-serif" font-size="18" fill="#7d8590" text-anchor="middle">AI & Robotics Enthusiast</text>
  
  <!-- Terminal-like element -->
  <g transform="translate(250, 200)">
    <rect x="0" y="0" width="300" height="60" rx="8" fill="#0d1117" stroke="#30363d" stroke-width="1" opacity="0.8"/>
    <circle cx="15" cy="15" r="4" fill="#ff5f56"/>
    <circle cx="35" cy="15" r="4" fill="#ffbd2e"/>
    <circle cx="55" cy="15" r="4" fill="#27ca3f"/>
    <text x="15" y="40" font-family="'Courier New', monospace" font-size="12" fill="#58a6ff">~/projects/robot-brain$</text>
    <text x="180" y="40" font-family="'Courier New', monospace" font-size="12" fill="#e6edf3">python main.py</text>
    <rect x="280" y="32" width="8" height="14" fill="#58a6ff" class="terminal-cursor"/>
  </g>
  
  <!-- Decorative elements -->
  <g opacity="0.6">
    <!-- Python logo inspired -->
    <circle cx="120" cy="150" r="8" fill="#3776ab"/>
    <circle cx="135" cy="150" r="8" fill="#ffd43b"/>
    
    <!-- C++ inspired -->
    <text x="650" y="120" font-family="'Arial Black', sans-serif" font-size="20" fill="#00599c" opacity="0.7">C++</text>
    
    <!-- Robot icon -->
    <g transform="translate(680, 150)">
      <rect x="0" y="0" width="20" height="15" rx="3" fill="#79c0ff" opacity="0.6"/>
      <circle cx="5" cy="5" r="2" fill="#0d1117"/>
      <circle cx="15" cy="5" r="2" fill="#0d1117"/>
      <rect x="8" y="10" width="4" height="3" fill="#0d1117"/>
    </g>
  </g>
  
  <!-- Connecting lines -->
  <path d="M100 150 Q200 150 250 180" stroke="#58a6ff" stroke-width="2" fill="none" opacity="0.3"/>
  <path d="M550 180 Q650 150 700 150" stroke="#f78166" stroke-width="2" fill="none" opacity="0.3"/>
</svg>

---

###  Who Am I?
- name: Izzul Fahmi
- role: AI & Robotics Enthusiast 
- focus: "AI/ML", "Robotics", "Embedded Systems"
- current_status: Student & Innovator
- fun_fact: I dream in Python and wake up debugging C++

###  My Mission
Building intelligent systems that bridge the gap between **artificial intelligence** and **real-world applications**. I'm passionate about creating robots that can truly understand and interact with their environment using cutting-edge LLM technology.

**Currently obsessed with:** Making AI accessible on resource-constrained devices!

---

## 🛠️ Tech Arsenal

###  Languages & Frameworks
<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

</div>

###  AI & ML Tools
<div align="center">

![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-FFD21E?style=for-the-badge)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=OpenCV&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)

</div>

###  Hardware & Systems
<div align="center">

![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=for-the-badge&logo=raspberry-pi&logoColor=white)
![ROS](https://img.shields.io/badge/ROS2-22314E?style=for-the-badge&logo=ros&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

</div>

###  Specialized Skills

**AI/ML Expertise:**
- LLM Fine-tuning (LoRA/QLoRA)
- Computer Vision (YOLO/MediaPipe) 
- Voice AI (Whisper/TTS)
- Transformer Architectures

**Robotics:**
- ROS2 Navigation
- Sensor Fusion
- Motion Planning
- Robot Middleware

**Systems:**
- Embedded Linux
- Real-time Processing
- Edge Computing
- SBC Optimization

---

### 🤖 **Autonomous LLM-Powered Robot Brain**

> **Vision:** Creating truly intelligent robots that can operate offline with human-like understanding

**🔍 What makes it special:**
- **Local LLM Integration** - Runs entirely offline on SBCs
- **Multimodal Perception** - Vision, audio, and sensor fusion  
- **Natural Communication** - Voice interaction with context awareness
- **Real-time Processing** - Optimized for edge computing
- **Modular Architecture** - Plug-and-play components

**Tech Stack:** Python, PyTorch, ROS2, OpenCV, Whisper, Custom LoRA models

**Status:** Currently in development | **Looking for:** Collaborators and feedback!

---

## 📊 GitHub Analytics

<div align="center">

<picture>
  <source media="(max-width: 600px)" srcset="https://github-readme-stats.vercel.app/api?username=IzzulGod&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&border_radius=10">
  <img src="https://github-readme-stats.vercel.app/api?username=IzzulGod&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&border_radius=10" alt="GitHub Stats">
</picture>

<picture>
  <source media="(max-width: 600px)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=IzzulGod&layout=compact&langs_count=6&theme=tokyonight&hide_border=true&border_radius=10&hide=html,css,scss">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=IzzulGod&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&border_radius=10&hide=html,css,scss" alt="Top Languages">
</picture>

</div>

<div align="center">

![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=IzzulGod&theme=tokyo-night&hide_border=true&radius=10)

</div>

---

## 🎮 Beyond Code

**Interests:** 
- Competitive Programming 
- AI Research Papers 
- Hardware Tinkering 
- Open Source Contributing

**Learning:** 
- Advanced Robotics 
- Transformer Architectures 
- Edge AI Optimization 
- Quantum Computing Basics  

**Gaming:** 
- Strategy Games 
- FPS & RPG 
- Indie Games 
- Mobile Gaming

---

### 💬 Open to discuss:
- **AI/ML Projects** 
- **Robotics Collaboration** 
- **Tech Innovation** 
- **Gaming** 
- **Learning Together**

---

<div align="center">

*"The future belongs to those who combine artificial intelligence with human creativity"* ✨
