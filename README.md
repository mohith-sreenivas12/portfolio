
# Mohith Sreenivas – Personal Portfolio Documentation  
 
GitHub Repository: https://github.com/mohith-sreenivas12/your-portfolio  

# Overview
This is a modern, visually striking, fully responsive single-page personal portfolio built with pure HTML5 and CSS3 (no JavaScript frameworks). It includes animated gradients, glassmorphism, floating dock navigation, hover effects, and smooth scrolling. 

The design showcases full-stack development skills with a cyberpunk/neon aesthetic.

### Tech Stack
| Technology        | Purpose                          |
|-------------------|----------------------------------|
| HTML5             | Semantic structure               |
| CSS3              | Animations and styling           |
| Google Fonts      | Poppins, Nosifer (horror-style)  |
| DevIcons CDN      | Skill icons                      |
| Font Awesome      | Dock navigation icons            |
| Pure CSS Animations | No JavaScript needed           |

# Key Features & Design Highlights

| Feature                       | Implementation Details                                                                |
|-------------------------------|----------------------------------------------------------------------------------------|
| Animated Gradient Background  | Two large blurred circles moving in moveVertical and moveInCircle animations           |
| Glassmorphism Cards           | backdrop-filter: blur() with semi-transparent backgrounds                              |
| Floating Dock Navigation      | Inspired by macOS dock with hover scale and glow effects                               |
| Gradient Text Effects         | -webkit-background-clip: text with animated linear gradients                           |
| Interactive Section Hover     | Cards lift, scale, and reveal animated gradient overlays on hover                      |
| Skill Icons Grid              | Responsive grid with hover scale and drop-shadow effects                               |
| Smooth Scrolling              | scroll-behavior: smooth with anchor links                                              |
| Mobile-First Responsive       | Fully responsive layout for phones and tablets                                         |
| Back-to-Top Button            | Floating arrow with GIF animation                                                      |

#File Structure

portfolio/
├── MyPortfolio.html           Main HTML file
├── styles.css                 All styling and animations
├── cvweb.pdf                  Downloadable resume
├── user.png                   Favicon
├── linkedin.png               Social icon
├── OIP.pmg.webp               GitHub icon
├── image.png                  Naukri.com icon
└── README.md                  This documentation


### CSS Architecture Explained

# 1. Root Variables & Global Reset
css
:root {
  --primary-color: #ff0000;
  --text-color: #ffffff;
  --shadow: complex multi-layer shadow;
}
* { margin:0; padding:0; box-sizing:border-box; }

# 2. Dynamic Gradient Background
css
.gradient-bg::before { animation: moveVertical 30s infinite; }
.gradient-bg::after  { animation: moveInCircle 20s reverse infinite; }

This creates a lively background that feels dynamic.

# 3. Animated Header Text
css
.header1 { 
  background: linear-gradient(to right, crimson, hotpink, blue);
  -webkit-background-clip: text;
  animation: textShine 5s infinite;
}


# 4. Floating Dock (Best Feature)
css
.floating-dock {
  backdrop-filter: blur(16px) saturate(180%);
  border-radius: 50px;
  position: fixed;
}
.dock-item:hover {
  transform: translateY(-3px) scale(1.03);
}

This is a pure CSS macOS-style dock with a glass effect.

# 5. Interactive Sections
`css
.section:hover {
  transform: scale(1.02) translateY(-5px);
  box-shadow: 0 20px 40px rgba(138,43,226,0.3);
}
.section::before { animated gradient overlay on hover }


# 6. Skill Cards with Glow
css
.skill-item:hover img {
  transform: scale(1.2);
  filter: drop-shadow(0 0 5px white);
}


#Color Palette
| Color           | Hex       | Usage                          |
|-----------------|-----------|--------------------------------|
| Deep Black      | #000000   | Base background                |
| Crimson Red     | #dc143c   | Primary accents                |
| Neon Pink       | #fb0303   | Gradient text                  |
| Electric Blue   | #081fce   | Secondary accents              |
| Gold            | #FFD700   | Headings and highlights        |
| White Smoke     | #f8f8f8   | Text and borders               |



# Responsive Breakpoints

| Device       | Key Changes                                      |
|--------------|--------------------------------------------------|
| ≤768px       | Dock moves to bottom and header font shrinks     |
| ≤480px       | Skills grid becomes 2-3 columns, padding reduced |
| Mobile       | Touch-friendly hover effects still work          |



# Accessibility Features
- Proper semantic HTML with elements like header, nav, main, and section
- aria-label on all important links
- High contrast text
- Focus indicators for keyboard navigation
- Smooth scrolling for better user experience



# Performance Optimizations
- Uses CDN-hosted icons for fast loading
- No external JavaScript for instant loading
- Efficient CSS animations using only transform and opacity
- Minimal HTTP requests



# How to Customize (For Future You)

| Want to Change          | Edit Here                                 |
|-------------------------|-------------------------------------------|
| Name & Title            | .header1 and #welcome in HTML             |
| Color Theme             | Update :root variables                    |
| Add New Skill           | Add new <div class="skill-item">          |
| Change Background Speed  | Modify animation durations in @keyframes |
| New Section             | Copy a .section block                     |
|


# Deployment Options (Free & Easy)

| Platform      | One-Click Deploy Link             |
|---------------|-----------------------------------|
| Vercel        | Drop folder to vercel.app         |
| Netlify       | Drag and drop to netlify.app      |
| GitHub Pages  | Settings, then Pages, then Deploy |

  
                                                                                        Made by Mohith Sreenivas Policherla  
                                                                                Full-Stack Developer | Java | Spring Boot | React | Open to opportunities




