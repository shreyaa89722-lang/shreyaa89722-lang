<svg width="650" height="390" viewBox="0 0 650 390" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bar1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#6C3483"/>
      <stop offset="100%" stop-color="#D7BDE2"/>
    </linearGradient>
    <linearGradient id="bar2" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#8E44AD"/>
      <stop offset="100%" stop-color="#C39BD3"/>
    </linearGradient>
    <linearGradient id="bar3" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#9B59B6"/>
      <stop offset="100%" stop-color="#E8DAEF"/>
    </linearGradient>
    <linearGradient id="bar4" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#76448A"/>
      <stop offset="100%" stop-color="#BB8FCE"/>
    </linearGradient>
    <linearGradient id="bar5" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#5B2C6F"/>
      <stop offset="100%" stop-color="#A569BD"/>
    </linearGradient>

    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <style>
      .label { font-family: 'Segoe UI', Verdana, sans-serif; font-size: 16px; fill: #E8DAEF; font-weight: 600; }
      .pct   { font-family: 'Segoe UI', Verdana, sans-serif; font-size: 14px; fill: #D7BDE2; }
      .track { fill: #1a1a1a; }
    </style>
  </defs>

  <rect width="650" height="390" fill="#000000"/>
  <text x="20" y="35" font-family="Segoe UI, sans-serif" font-size="20" font-weight="700" fill="#9B59B6">🎯 Current Learning Progress</text>

  <!-- Python 80% -->
  <text x="20" y="80" class="label">🐍 Python</text>
  <rect x="20" y="90" width="590" height="16" rx="8" class="track"/>
  <rect x="20" y="90" width="472" height="16" rx="8" fill="url(#bar1)" filter="url(#glow)">
    <animate attributeName="width" from="0" to="472" dur="1.2s" fill="freeze"/>
  </rect>
  <text x="620" y="103" class="pct" text-anchor="end">80%</text>

  <!-- Pandas 70% -->
  <text x="20" y="140" class="label">🐼 Pandas</text>
  <rect x="20" y="150" width="590" height="16" rx="8" class="track"/>
  <rect x="20" y="150" width="413" height="16" rx="8" fill="url(#bar2)" filter="url(#glow)">
    <animate attributeName="width" from="0" to="413" dur="1.2s" fill="freeze"/>
  </rect>
  <text x="620" y="163" class="pct" text-anchor="end">70%</text>

  <!-- SQL 60% -->
  <text x="20" y="200" class="label">🗄️ SQL</text>
  <rect x="20" y="210" width="590" height="16" rx="8" class="track"/>
  <rect x="20" y="210" width="354" height="16" rx="8" fill="url(#bar3)" filter="url(#glow)">
    <animate attributeName="width" from="0" to="354" dur="1.2s" fill="freeze"/>
  </rect>
  <text x="620" y="223" class="pct" text-anchor="end">60%</text>

  <!-- Data Viz 50% -->
  <text x="20" y="260" class="label">📊 Data Viz</text>
  <rect x="20" y="270" width="590" height="16" rx="8" class="track"/>
  <rect x="20" y="270" width="295" height="16" rx="8" fill="url(#bar4)" filter="url(#glow)">
    <animate attributeName="width" from="0" to="295" dur="1.2s" fill="freeze"/>
  </rect>
  <text x="620" y="283" class="pct" text-anchor="end">50%</text>

  <!-- AWS Cloud 20% -->
  <text x="20" y="320" class="label">☁️ AWS Cloud</text>
  <rect x="20" y="330" width="590" height="16" rx="8" class="track"/>
  <rect x="20" y="330" width="118" height="16" rx="8" fill="url(#bar5)" filter="url(#glow)">
    <animate attributeName="width" from="0" to="118" dur="1.2s" fill="freeze"/>
  </rect>
  <text x="620" y="343" class="pct" text-anchor="end">20%</text>
</svg>
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,100:6C3483&height=220&section=header&text=Hi%20there,%20I'm%20Shreya%20👋&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Aspiring%20Data%20Engineer%20·%20Python%20·%20SQL%20·%20Pandas&descAlignY=55&descSize=18&descColor=D7BDE2" width="100%"/>

<a href="https://www.linkedin.com/in/shreya-gn"><img src="https://img.shields.io/badge/LinkedIn-000000?style=flat-square&logo=linkedin&logoColor=9B59B6"/></a>
<a href="mailto:shreyaa89722@gmail.com"><img src="https://img.shields.io/badge/Email-000000?style=flat-square&logo=gmail&logoColor=9B59B6"/></a>
<a href="https://github.com/shreyaa89722-lang"><img src="https://img.shields.io/badge/GitHub-000000?style=flat-square&logo=github&logoColor=9B59B6"/></a>

</div>

<br>

## 💜 About Me

I'm a final-year **B.Tech student at Malnad College of Engineering**, based in Bengaluru, India 🇮🇳 — turning messy datasets into clean, usable pipelines and dashboards.

```yaml
role:        Aspiring Data Engineer
currently:   Building end-to-end data pipelines
learning:    SQL · Apache Airflow · AWS Cloud
goal:        Land a Data Engineering internship 🎯
fun_fact:    I code better at night 🌙
```

<br>

## 🛠️ Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=python,mysql,sqlite,jupyter,vscode,git,github,aws&theme=dark" />

</div>

<br>

## 🚀 Featured Projects

<table>
<tr>
<td width="33%" valign="top">

### 🎮 Gaming Sales Analytics
Analysed **16,000+** video game sales records to uncover industry trends — top sellers, platforms, genres, and revenue by publisher.

`Python` `Pandas` `Matplotlib`

**[View Project →](https://github.com/shreyaa89722-lang/gaming-analytics-pipeline)**

</td>
<td width="33%" valign="top">

### 🎬 YouTube Trending Pipeline
Analysed **40,000+** trending videos to find what drives virality — best upload times, top channels, views-vs-likes patterns.

`Python` `SQLite` `SQL`

**[View Project →](https://github.com/shreyaa89722-lang/youtube-trends-pipeline)**

</td>
<td width="33%" valign="top">

### 🛒 E-Commerce Sales Analytics
Processed **180,000+** orders to surface revenue trends — best month/city for sales, top products, ideal ad timing.

`Python` `SQL` `Matplotlib`

**[View Project →](https://github.com/shreyaa89722-lang/ecommerce-sales-pipeline)**

</td>
</tr>
</table>

<br>

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=shreyaa89722-lang&show_icons=true&theme=midnight-purple&hide_border=true&count_private=true&bg_color=000000&title_color=9B59B6&icon_color=9B59B6" width="49%"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=shreyaa89722-lang&layout=compact&theme=midnight-purple&hide_border=true&bg_color=000000&title_color=9B59B6" width="35%"/>

<br>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=shreyaa89722-lang&theme=midnight-purple&hide_border=true&background=000000&stroke=9B59B6&ring=9B59B6&fire=D7BDE2&currStreakLabel=D7BDE2" width="70%"/>

</div>

<br>

<div align="center">

<img src="https://raw.githubusercontent.com/shreyaa89722-lang/shreyaa89722-lang/main/assets/progress-bars.svg" width="100%"/>

</div>

<br>

<div align="center">

### 💜 *"Data is the new oil — I refine it."*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6C3483,100:000000&height=120&section=footer" width="100%"/>

</div>
