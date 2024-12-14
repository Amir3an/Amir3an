# 💻 > Hey There!, I am AmirAli

I am a **front-end developer** with **2 years of experience**, specializing in **Vue.js**, **HTML/CSS**, and **Tailwind CSS**. I enjoy crafting professional and efficient user interfaces and am currently working on projects like **corporate websites** and **management panels**. 🌟

---

## 👨‍💻 About Me
- 🔥 **16 years old** and studying in **technical high school**  
- 🎯 Goal: To deepen and professionalize my web development skills  
- 🌎 Based in **Iran**  
- ☕ A single shot of espresso fuels my daily coding sessions! 😄  
- 📝 Proficient in **English reading and writing**

---

## ✨ Skills  
### Front-End Development  
- Vue.js  
- Tailwind CSS  
- JavaScript (Frameworks and DOM Manipulation)  
- HTML & CSS (Responsive and professional design)  
- Beginner-level experience with WordPress

---

## 🏆 Achievements & Projects  
1. **Corporate Management Panel**  
   - Includes **data tables**, **varied menus**, and **dual-language support**  
   - Professionally structured and user-friendly

2. **Corporate Website**  
   - Integrated with **API** for dynamic data display  
   - Features a **dynamic news slider** using **Vue.js Swiper**

3. **Mini Projects:**  
   - **Family Tree**: Designed a tree structure using HTML and CSS  
   - **Responsive News Slider**

---

## 🌍 Contact Me  
- **GitHub:** [github.com/Amir3an](#)  
- **Instagram:** [instagram.com/amir_3an](#)  
- **Telegram:** [t.me/Amir3an](#)

---

## 📈 Future Goals  
- Mastering **JavaScript Core**  
- Enhancing scalability in web design  
- Contributing to open-source projects to support the developer community

---

## 📊 My Stats and Projects

### 1. **Skills Chart**
<canvas id="skillsChart" width="400" height="400"></canvas>

### 2. **Activity Chart**
<canvas id="activityChart" width="400" height="200"></canvas>

### 3. **Goals Progress**
<canvas id="goalChart" width="400" height="400"></canvas>

### 4. **Projects Completed**
<canvas id="projectsChart" width="400" height="200"></canvas>

### 5. **Goal Progress Example**
<div id="goal1" class="progress-bar"></div>

---

## 📈 Code for Charts and Progress Bar

### Chart.js Integration
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<script>
// Skills Chart
const ctx = document.getElementById('skillsChart').getContext('2d');
const skillsChart = new Chart(ctx, {
    type: 'doughnut',
    data: {
        labels: ['Vue.js', 'Tailwind CSS', 'JavaScript', 'HTML & CSS', 'WordPress'],
        datasets: [{
            label: 'Skill Proficiency',
            data: [90, 80, 70, 85, 40],
            backgroundColor: ['#3498db', '#2ecc71', '#f39c12', '#9b59b6', '#e74c3c'],
            borderWidth: 1
        }]
    }
});

// Activity Chart
const activityCtx = document.getElementById('activityChart').getContext('2d');
const activityChart = new Chart(activityCtx, {
    type: 'line',
    data: {
        labels: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul'],
        datasets: [{
            label: 'Coding Activity',
            data: [20, 30, 25, 50, 45, 55, 60],
            fill: false,
            borderColor: '#3498db',
            tension: 0.1
        }]
    }
});

// Goals Progress Chart
const goalCtx = document.getElementById('goalChart').getContext('2d');
const goalChart = new Chart(goalCtx, {
    type: 'doughnut',
    data: {
        labels: ['Master JavaScript', 'Open Source Contribution', 'Web Design Scalability'],
        datasets: [{
            label: 'Goal Progress',
            data: [70, 50, 40],
            backgroundColor: ['#e74c3c', '#f39c12', '#2ecc71'],
            borderWidth: 1
        }]
    }
});

// Projects Chart
const projectsCtx = document.getElementById('projectsChart').getContext('2d');
const projectsChart = new Chart(projectsCtx, {
    type: 'bar',
    data: {
        labels: ['Corporate Management Panel', 'Corporate Website', 'Mini Projects'],
        datasets: [{
            label: 'Projects Completed',
            data: [1, 1, 3],
            backgroundColor: '#3498db',
            borderColor: '#2980b9',
            borderWidth: 1
        }]
    }
});
</script>

### ProgressBar.js Integration
<script src="https://cdn.jsdelivr.net/npm/progressbar.js"></script>

<script>
const goal1 = new ProgressBar.Circle('#goal1', {
    color: '#3498db',
    strokeWidth: 6,
    duration: 1400,
    easing: 'easeInOut',
    from: { color: '#eee', width: 1 },
    to: { color: '#3498db', width: 6 },
    step: function(state, circle) {
        circle.path.setAttribute('stroke', state.color);
        circle.path.setAttribute('stroke-width', state.width);
        circle.setText(Math.round(circle.value() * 100) + ' %');
    }
});

goal1.animate(0.7);  // Goal progress at 70%
</script>
