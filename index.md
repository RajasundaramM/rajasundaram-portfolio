---
layout: home # Or 'page' - 'home' is semantically good for a homepage
title: Rajasundaram's Robotics Portfolio
permalink: /
---

<div class="home-hero" style="background-image: url('/assets/img/profile.jpg');">
  <div class="home-hero-content">
    <h1>Rajasundaram Mathiazhagan</h1>
    <p class="lead">Robotics • Perception • AI</p>
    <p>Innovating at the intersection of intelligent autonomous systems.</p>
    <div class="mt-5">
      <a href="#welcome-section" class="btn btn-primary">
        <i class="fas fa-angle-down me-2"></i>Learn More
      </a>
      <a href="{{ '/projects/' | relative_url }}" class="btn btn-secondary">
        <i class="fas fa-rocket me-2"></i>View Projects
      </a>
    </div>
  </div>
  <a href="#welcome-section" class="scroll-down">
    <i class="fas fa-chevron-down"></i>
  </a>
</div>

<div class="container-fluid content-section" id="welcome-section">
  <div class="row justify-content-center">
    <div class="col-md-9 col-lg-8 text-center">
      <h2>Welcome to My Portfolio!</h2>
      <p class="lead">
        I'm **Rajasundaram Mathiazhagan**, a passionate Robotics Engineer with a strong background in **autonomy, perception, and intelligent systems**. My journey in robotics began with a fascination for creating machines that can sense, understand, and interact with the world around them.
      </p>
      <p>
        Explore my work in **Robot Perception**, **Control**, and **AI applications**.
      </p>
    </div>
  </div>
</div>

<div class="container-fluid content-section" id="about-me-section">
  <div class="row justify-content-center">
    <div class="col-md-9 col-lg-8">
      <h2 class="text-center">About Me</h2>
      <p>Throughout my academic and professional career, I've focused on developing robust and efficient solutions for complex robotics challenges. My expertise spans across areas like:</p>
      <ul>
        <li><strong>Robot Perception:</strong> LiDAR and Camera-based object detection, tracking, and 3D reconstruction.</li>
        <li><strong>Motion Planning & Control:</strong> Kinematics, dynamics, path planning, and trajectory optimization for robotic manipulators and mobile robots.</li>
        <li><strong>Artificial Intelligence:</strong> Applying machine learning and deep learning techniques for robotic decision-making and cognitive tasks.</li>
        <li><strong>Software Development:</strong> Proficient in C++ and Python for real-time systems and algorithm implementation, often utilizing ROS (Robot Operating System).</li>
      </ul>
      <p>I'm driven by the goal of contributing to the next generation of autonomous systems that can safely and intelligently operate in various environments, from industrial settings to everyday human spaces. I thrive on problem-solving, enjoy collaborative environments, and am always eager to learn and adapt to new technologies.</p>
      <p>This portfolio showcases a selection of my **projects** and **experiences**, highlighting my technical skills and passion for bringing intelligent robots to life. Feel free to explore and connect!</p>
    </div>
  </div>
</div>

<div class="container-fluid content-section text-center">
  <div class="row justify-content-center">
    <div class="col-md-9 col-lg-8">
      <h2>Featured Projects</h2>
      <p class="lead">Dive into some of my key innovations and contributions.</p>
      <div class="row mt-5">
        <div class="col-md-6 mb-4">
          <div class="card h-100 shadow-sm">
            <img src="{{ '/assets/img/profile.jpg' | relative_url }}" class="card-img-top" alt="Project 1">
            <div class="card-body">
              <h5 class="card-title">Project Title 1</h5>
              <p class="card-text">A brief description of your first featured project.</p>
              <a href="{{ '/projects/project-1/' | relative_url }}" class="btn btn-outline-primary">Learn More</a>
            </div>
          </div>
        </div>
        <div class="col-md-6 mb-4">
          <div class="card h-100 shadow-sm">
            <img src="{{ '/assets/img/profile.jpg' | relative_url }}" class="card-img-top" alt="Project 2">
            <div class="card-body">
              <h5 class="card-title">Project Title 2</h5>
              <p class="card-text">A brief description of your second featured project.</p>
              <a href="{{ '/projects/project-2/' | relative_url }}" class="btn btn-outline-primary">Learn More</a>
            </div>
          </div>
        </div>
      </div>
      <p class="mt-4"><a href="{{ '/projects/' | relative_url }}" class="btn btn-lg btn-info">Explore All Projects <i class="fas fa-arrow-right ms-2"></i></a></p>
    </div>
  </div>
</div>
