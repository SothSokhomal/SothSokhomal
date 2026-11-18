<div align="center">

<img src="banner.svg" alt="Soth Vannak RothChansokhomal, also known as ByteBabe. Software Engineering Student and Full-Stack Developer" width="100%"/>

### Software engineering student building full-stack web and mobile products with React, Node.js and Flutter.

Based in Phnom Penh, Cambodia 🌸

[![Portfolio](https://img.shields.io/badge/Portfolio-E8789F?style=for-the-badge)](https://www.sothsokhomal.com/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-B8A1E3?style=for-the-badge)](https://www.linkedin.com/in/sothvannakrothchansokhomal/)
[![Email](https://img.shields.io/badge/Email-F4A6C0?style=for-the-badge&logo=gmail&logoColor=4A2545)](mailto:soth.vannakrothchansokhomal@gmail.com)

</div>

<br/>

<table align="center">
  <tr>
    <td align="center" width="33%">🥈<br/><b>First Runner-Up</b><br/><sub>E-Gen Innovation Program, MoEYS (2025)</sub></td>
    <td align="center" width="33%">🏅<br/><b>Top 5 Finalist</b><br/><sub>SEA Sponge City Innovation Challenge (2025)</sub></td>
    <td align="center" width="33%">🛰️<br/><b>NASA Space Apps Challenge</b><br/><sub>ORBY, a space-exploration game with real NASA data</sub></td>
  </tr>
</table>

---

## ✨ About

I am a second-year Software Engineering student at CamTech. I build practical software: reliable backend services, clear interfaces, and products that work for the people who use them. I work well in teams and I care about accessibility, especially for communities with limited internet access.

| | |
|---|---|
| 💬 **Languages** | Khmer (native), English (fluent) |
| 🌱 **Looking for** | Software engineering internships (full-stack and backend) |

## 🧭 How I Work in the Era of AI

AI helps me build faster, but good software still starts with people. This is the order I follow:

1. **Know the problem from the user.** I start with the people who will use the product.
2. **Plan the project with the SDLC.** I follow the Software Development Life Cycle and write every document the user's requirements call for.
3. **Design the whole system.** I plan the system design and the architecture of the full system.
4. **Design the UX/UI.** I shape the experience and the interface before the build.

### The six stages

| # | Stage | What I do | Key deliverables |
|---|---|---|---|
| 01 | **Problem Discovery**<br/><sub>Empathize and frame</sub> | Identify real-world friction points, user frustrations and technical constraints before writing a single line of code. | User interviews, problem definition, scope mapping |
| 02 | **Research and Insights**<br/><sub>Explore and analyze</sub> | Analyze existing solutions, survey target audiences and form data-backed architectural hypotheses. | Competitive auditing, user personas, feature matrix |
| 03 | **UX Architecture**<br/><sub>Structure and flow</sub> | Map user journeys and information architecture, and set up scalable database schemas and API contracts. | Wireframing, user flowcharts, API contract specs |
| 04 | **UI Design and Prototyping**<br/><sub>Design and iterate</sub> | Craft design systems in Figma with tokens, typography hierarchy, high contrast and interactive prototypes. | Design system tokens, Figma high-fidelity mockups, interactive prototypes |
| 05 | **Agile Engineering**<br/><sub>Develop and test</sub> | Translate designs into clean TypeScript and React code with full modularity, state management and edge-case testing. | React / Next.js implementation, Node.js API integration, unit and end-to-end validation |
| 06 | **Ship and Iterate**<br/><sub>Deploy and optimize</sub> | Deploy to cloud platforms, evaluate Core Web Vitals and keep gathering user feedback for continuous improvement. | Production CI/CD, performance tuning, post-launch analytics |

### System architecture: shaped by the project

I do not use one fixed architecture. I start from the same layers (clients, backend, data and services) and keep only what each project needs.

<details open>
<summary><b>📚 Jomnes App</b>: mobile app with a REST API</summary>

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'primaryColor': '#FFE6F0', 'primaryBorderColor': '#E8789F', 'primaryTextColor': '#4A2545', 'lineColor': '#B0558A', 'clusterBkg': '#F6EAF2', 'clusterBorder': '#B8A1E3'}}}%%
flowchart LR
  subgraph Client["Client"]
    App["Flutter app<br/>students and parents"]
  end
  subgraph Backend["Backend"]
    API["REST API<br/>Node.js / Express.js<br/>teacher discovery and filters"]
  end
  subgraph Data["Data"]
    DB[("Supabase<br/>tutor profiles")]
  end
  App --> API
  API --> DB
```

</details>

<details>
<summary><b>🌐 Portfolio Website with Admin Portal</b>: public site, admin area and Telegram bot</summary>

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'primaryColor': '#FFE6F0', 'primaryBorderColor': '#E8789F', 'primaryTextColor': '#4A2545', 'lineColor': '#B0558A', 'clusterBkg': '#F6EAF2', 'clusterBorder': '#B8A1E3'}}}%%
flowchart LR
  Visitor(("Recruiter"))
  Owner(("Admin"))
  subgraph Clients["Clients"]
    Site["React site<br/>case studies and contact form"]
    Portal["Admin portal"]
  end
  subgraph Backend["Backend"]
    API["API<br/>Node.js / Express.js"]
  end
  Bot["Telegram bot"]
  Visitor --> Site
  Owner --> Portal
  Site --> API
  Portal --> API
  API --- Bot
```

</details>

<details>
<summary><b>🌦️ AI-Powered Weather Chatbot</b>: conversational interface with NLP and live data</summary>

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'primaryColor': '#FFE6F0', 'primaryBorderColor': '#E8789F', 'primaryTextColor': '#4A2545', 'lineColor': '#B0558A', 'clusterBkg': '#F6EAF2', 'clusterBorder': '#B8A1E3'}}}%%
flowchart LR
  User(("User"))
  subgraph Client["Client"]
    UI["React interface"]
  end
  subgraph Backend["Backend"]
    Server["Node.js server"]
    NLP["NLP<br/>intent recognition"]
  end
  subgraph Services["External service"]
    Weather["OpenWeatherMap API<br/>live weather data"]
  end
  User --> UI
  UI --> Server
  Server --> NLP
  Server --> Weather
```

</details>

<details>
<summary><b>🏠 HomeSweet Rental App</b>: cross-platform clients on Firebase</summary>

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'primaryColor': '#FFE6F0', 'primaryBorderColor': '#E8789F', 'primaryTextColor': '#4A2545', 'lineColor': '#B0558A', 'clusterBkg': '#F6EAF2', 'clusterBorder': '#B8A1E3'}}}%%
flowchart LR
  subgraph Clients["Clients"]
    Flutter["Flutter app"]
    Vue["Vue.js app"]
  end
  subgraph BaaS["Backend as a service"]
    FB[("Firebase")]
  end
  Flutter --> FB
  Vue --> FB
```

</details>

<details>
<summary><b>🚀 ORBY</b>: web game with real NASA data</summary>

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'primaryColor': '#FFE6F0', 'primaryBorderColor': '#E8789F', 'primaryTextColor': '#4A2545', 'lineColor': '#B0558A', 'clusterBkg': '#F6EAF2', 'clusterBorder': '#B8A1E3'}}}%%
flowchart LR
  Player(("Player"))
  subgraph App["ORBY web app<br/>TypeScript, hosted on Vercel"]
    Game["Game mode<br/>lead 4 astronauts for 90 days"]
    Solar["Solar System mode<br/>explore planets and moons"]
  end
  NASA[("Real NASA data")]
  Player --> Game
  Player --> Solar
  Solar --> NASA
```

</details>

<details>
<summary><b>🧩 Full reference architecture</b>: every layer I can combine</summary>

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'primaryColor': '#FFE6F0', 'primaryBorderColor': '#E8789F', 'primaryTextColor': '#4A2545', 'lineColor': '#B0558A', 'clusterBkg': '#F6EAF2', 'clusterBorder': '#B8A1E3'}}}%%
flowchart LR
  subgraph Clients
    Web["Web<br/>React / Vue / PWA"]
    Desktop["Desktop<br/>Electron"]
    Mobile["Mobile<br/>Flutter / Expo"]
  end
  subgraph Backend
    RT["Real-time<br/>Socket.IO"]
    API["REST API<br/>Express / FastAPI"]
  end
  subgraph Data
    FB[("Firebase")]
    PG[("PostgreSQL<br/>Neon / Supabase")]
  end
  subgraph Services
    Pay["Payments<br/>ABA KHQR"]
    OCR["OCR + TTS<br/>Vision / Azure"]
    POS["Brokers + POS<br/>MT5 / Loyverse"]
    AI["AI<br/>Gemini / Ollama"]
  end
  Web --> FB
  Web --> PG
  Web <--> RT
  Web --> API
  Desktop --> API
  Mobile --> API
  API --> PG
  API --> Pay
  API --> OCR
  API --> POS
  API --> AI
```

</details>

---

## 🎀 Tech Stack

**Languages**
![TypeScript](https://img.shields.io/badge/TypeScript-F4A6C0?style=flat-square&logo=typescript&logoColor=4A2545)
![JavaScript](https://img.shields.io/badge/JavaScript-F4A6C0?style=flat-square&logo=javascript&logoColor=4A2545)
![Dart](https://img.shields.io/badge/Dart-F4A6C0?style=flat-square&logo=dart&logoColor=4A2545)
![Python](https://img.shields.io/badge/Python-F4A6C0?style=flat-square&logo=python&logoColor=4A2545)
![Java](https://img.shields.io/badge/Java-F4A6C0?style=flat-square&logo=openjdk&logoColor=4A2545)
![C/C++](https://img.shields.io/badge/C%2FC%2B%2B-F4A6C0?style=flat-square&logo=cplusplus&logoColor=4A2545)

**Web and backend**
![React](https://img.shields.io/badge/React-D9CCF7?style=flat-square&logo=react&logoColor=4A2545)
![Node.js](https://img.shields.io/badge/Node.js-D9CCF7?style=flat-square&logo=nodedotjs&logoColor=4A2545)
![Express](https://img.shields.io/badge/Express-D9CCF7?style=flat-square&logo=express&logoColor=4A2545)
![Telegram Bot](https://img.shields.io/badge/Telegram_Bot-D9CCF7?style=flat-square&logo=telegram&logoColor=4A2545)
![REST API](https://img.shields.io/badge/REST_API-D9CCF7?style=flat-square)
![HTML5](https://img.shields.io/badge/HTML5-D9CCF7?style=flat-square&logo=html5&logoColor=4A2545)
![CSS3](https://img.shields.io/badge/CSS3-D9CCF7?style=flat-square&logo=css3&logoColor=4A2545)
![Bootstrap](https://img.shields.io/badge/Bootstrap-D9CCF7?style=flat-square&logo=bootstrap&logoColor=4A2545)

**AI and computer vision**
![OpenCV](https://img.shields.io/badge/OpenCV-FFD6E7?style=flat-square&logo=opencv&logoColor=4A2545)
![NLP](https://img.shields.io/badge/NLP-FFD6E7?style=flat-square)

**Mobile**
![Flutter](https://img.shields.io/badge/Flutter-FFD6E7?style=flat-square&logo=flutter&logoColor=4A2545)

**Databases and platforms**
![MySQL](https://img.shields.io/badge/MySQL-FFE6F0?style=flat-square&logo=mysql&logoColor=4A2545)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-FFE6F0?style=flat-square&logo=postgresql&logoColor=4A2545)
![MongoDB](https://img.shields.io/badge/MongoDB-FFE6F0?style=flat-square&logo=mongodb&logoColor=4A2545)
![Prisma](https://img.shields.io/badge/Prisma-FFE6F0?style=flat-square&logo=prisma&logoColor=4A2545)
![Supabase](https://img.shields.io/badge/Supabase-FFE6F0?style=flat-square&logo=supabase&logoColor=4A2545)
![Firebase](https://img.shields.io/badge/Firebase-FFE6F0?style=flat-square&logo=firebase&logoColor=4A2545)

**Tools and practices**
![Git](https://img.shields.io/badge/Git-E9DDFB?style=flat-square&logo=git&logoColor=4A2545)
![GitHub](https://img.shields.io/badge/GitHub-E9DDFB?style=flat-square&logo=github&logoColor=4A2545)
![Postman](https://img.shields.io/badge/Postman-E9DDFB?style=flat-square&logo=postman&logoColor=4A2545)
![Jira](https://img.shields.io/badge/Jira-E9DDFB?style=flat-square&logo=jira&logoColor=4A2545)
![Trello](https://img.shields.io/badge/Trello-E9DDFB?style=flat-square&logo=trello&logoColor=4A2545)
![Figma](https://img.shields.io/badge/Figma-E9DDFB?style=flat-square&logo=figma&logoColor=4A2545)
![Canva](https://img.shields.io/badge/Canva-E9DDFB?style=flat-square&logo=canva&logoColor=4A2545)
![OOP](https://img.shields.io/badge/OOP-E9DDFB?style=flat-square)
![Agile/Scrum](https://img.shields.io/badge/Agile%2FScrum-E9DDFB?style=flat-square)
![UX/UI](https://img.shields.io/badge/UX%2FUI_Design-E9DDFB?style=flat-square)

---

<h1 align="center">🌸 Featured Projects 🌸</h1>

<p align="center">Selected work across engineering, innovation and community impact.</p>

<br/>

<h2 align="center">💻 Engineering</h2>

<p align="center"><sub>Full-stack, mobile and computer vision work</sub></p>

<!-- TODO: add your role in ORBY and the Space Apps result to the ORBY card -->
<!-- TODO: say what the admin portal manages and what the Telegram bot does -->
<!-- TODO: add the Jomnes live demo and GitHub repository links once they are public -->
<table width="100%">
<tr>
<td width="50%" valign="top">
<img alt="Engineering" src="https://img.shields.io/badge/Engineering-E8789F?style=flat-square"/> <img alt="NASA Space Apps" src="https://img.shields.io/badge/NASA_Space_Apps-B8A1E3?style=flat-square"/>
<h3>🚀 ORBY</h3>
<b>Lunar astronaut training game</b>
<p>An interactive space-exploration game built for the NASA Space Apps Challenge.</p>
<ul>
<li><b>What it does:</b> Players lead a crew of four astronauts at the Lunar South Pole for 90 days (Project Artemis) and explore planets and moons with real NASA data.</li>
<li><b>Features:</b> Missions, a leaderboard and crew screens.</li>
</ul>
<p><img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-D9CCF7?style=flat-square"/></p>
<p><a href="https://orby-project.vercel.app/"><img alt="Live Demo" src="https://img.shields.io/badge/Live_Demo-E8789F?style=flat-square"/></a> <a href="https://github.com/SothSokhomal/ORBY-Project"><img alt="Source Code" src="https://img.shields.io/badge/Source_Code-B8A1E3?style=flat-square"/></a></p>
</td>
<td width="50%" valign="top">
<img alt="Engineering" src="https://img.shields.io/badge/Engineering-E8789F?style=flat-square"/> <img alt="Full-stack" src="https://img.shields.io/badge/Full--stack-B8A1E3?style=flat-square"/>
<h3>🌐 Portfolio Website with Admin Portal</h3>
<b>Personal site for recruiters</b>
<p>A portfolio that gives recruiters one place to see my skills, projects and experience.</p>
<ul>
<li><b>What it does:</b> Presents each project as a case study, along with skills, experience, a downloadable résumé and a contact form.</li>
<li><b>Admin portal:</b> A separate admin portal for managing the site.</li>
<li><b>Telegram bot:</b> A Telegram bot connected to the site.</li>
</ul>
<p><img alt="React" src="https://img.shields.io/badge/React-D9CCF7?style=flat-square"/> <img alt="Node.js" src="https://img.shields.io/badge/Node.js-D9CCF7?style=flat-square"/> <img alt="Express.js" src="https://img.shields.io/badge/Express.js-D9CCF7?style=flat-square"/> <img alt="Telegram Bot" src="https://img.shields.io/badge/Telegram_Bot-D9CCF7?style=flat-square"/></p>
<p><a href="https://www.sothsokhomal.com/"><img alt="Live Site" src="https://img.shields.io/badge/Live_Site-E8789F?style=flat-square"/></a></p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<img alt="Engineering" src="https://img.shields.io/badge/Engineering-E8789F?style=flat-square"/> <img alt="NLP" src="https://img.shields.io/badge/NLP-B8A1E3?style=flat-square"/>
<h3>🌦️ AI-Powered Weather Chatbot</h3>
<b>Conversational weather assistant</b>
<p>A chatbot that answers real-time weather questions for any location.</p>
<ul>
<li><b>What I built:</b> An NLP chatbot with intent recognition, so it understands varied ways of asking, plus a React interface.</li>
<li><b>Integration:</b> OpenWeatherMap API for live weather data from the user's location query.</li>
</ul>
<p><img alt="React.js" src="https://img.shields.io/badge/React.js-D9CCF7?style=flat-square"/> <img alt="Node.js" src="https://img.shields.io/badge/Node.js-D9CCF7?style=flat-square"/> <img alt="NLP" src="https://img.shields.io/badge/NLP-D9CCF7?style=flat-square"/> <img alt="OpenWeatherMap API" src="https://img.shields.io/badge/OpenWeatherMap_API-D9CCF7?style=flat-square"/></p>
<p><a href="https://weather-ai-bot-632079387667.asia-southeast1.run.app/"><img alt="Live Demo" src="https://img.shields.io/badge/Live_Demo-E8789F?style=flat-square"/></a> <a href="https://github.com/SothSokhomal/Weather-Bot-App"><img alt="Source Code" src="https://img.shields.io/badge/Source_Code-B8A1E3?style=flat-square"/></a></p>
</td>
<td width="50%" valign="top">
<img alt="Engineering" src="https://img.shields.io/badge/Engineering-E8789F?style=flat-square"/> <img alt="Computer Vision" src="https://img.shields.io/badge/Computer_Vision-B8A1E3?style=flat-square"/>
<h3>🧑‍💻 Face Recognition</h3>
<b>Real-time computer vision pipeline</b>
<p>An end-to-end facial recognition pipeline.</p>
<ul>
<li><b>What I built:</b> A Python and OpenCV application that uses live webcam input to detect faces, draw bounding boxes and perform identity verification.</li>
</ul>
<p><img alt="Python" src="https://img.shields.io/badge/Python-D9CCF7?style=flat-square"/> <img alt="OpenCV" src="https://img.shields.io/badge/OpenCV-D9CCF7?style=flat-square"/></p>
<p><a href="https://github.com/SothSokhomal/Face_Recognition"><img alt="Source Code" src="https://img.shields.io/badge/Source_Code-E8789F?style=flat-square"/></a></p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<img alt="Engineering" src="https://img.shields.io/badge/Engineering-E8789F?style=flat-square"/> <img alt="Mobile" src="https://img.shields.io/badge/Mobile-B8A1E3?style=flat-square"/>
<h3>📚 Jomnes App</h3>
<b>Find part-time educators</b>
<p>A mobile app that helps students and parents find part-time educators.</p>
<ul>
<li><b>My role:</b> Backend developer in a team with Flutter developers.</li>
<li><b>What I built:</b> Node.js and Express.js REST APIs for teacher discovery, with filtering by subject, level, location and availability, plus structured tutor profiles covering subjects, pricing, schedule and contact details.</li>
<li><b>Collaboration:</b> Shared work with the Flutter developers through Git and GitHub.</li>
</ul>
<p><img alt="Flutter" src="https://img.shields.io/badge/Flutter-D9CCF7?style=flat-square"/> <img alt="Dart" src="https://img.shields.io/badge/Dart-D9CCF7?style=flat-square"/> <img alt="Node.js" src="https://img.shields.io/badge/Node.js-D9CCF7?style=flat-square"/> <img alt="Express.js" src="https://img.shields.io/badge/Express.js-D9CCF7?style=flat-square"/> <img alt="Supabase" src="https://img.shields.io/badge/Supabase-D9CCF7?style=flat-square"/></p>
</td>
<td width="50%" valign="top">
<img alt="Engineering" src="https://img.shields.io/badge/Engineering-E8789F?style=flat-square"/> <img alt="Cross-platform" src="https://img.shields.io/badge/Cross--platform-B8A1E3?style=flat-square"/>
<h3>🏠 HomeSweet Rental App</h3>
<b>Student housing app</b>
<p>A cross-platform student housing app.</p>
<ul>
<li><b>My role:</b> Lead designer and system architect. I led the design team and coordinated requirements with developers.</li>
<li><b>What I built:</b> System architecture diagrams, flowcharts and data flows, plus technical specifications and design documentation.</li>
</ul>
<p><img alt="Flutter" src="https://img.shields.io/badge/Flutter-D9CCF7?style=flat-square"/> <img alt="Vue.js" src="https://img.shields.io/badge/Vue.js-D9CCF7?style=flat-square"/> <img alt="Firebase" src="https://img.shields.io/badge/Firebase-D9CCF7?style=flat-square"/></p>
<p><a href="https://www.homesweet.site/"><img alt="Live Demo" src="https://img.shields.io/badge/Live_Demo-E8789F?style=flat-square"/></a></p>
</td>
</tr>
</table>

<br/>

<h2 align="center">🌍 Innovation and Impact</h2>

<p align="center"><sub>Climate resilience and inclusive technology in Cambodia</sub></p>

<table width="100%">
<tr>
<td width="33%" valign="top">
<img alt="Innovation" src="https://img.shields.io/badge/Innovation-B8A1E3?style=flat-square"/> <img alt="UX Research" src="https://img.shields.io/badge/UX_Research-FFD6E7?style=flat-square"/>
<h3>🌫️ ClearAir</h3>
<b>Emergency air-pollution alert app</b>
<p>Real-time air quality alerts for people exposed to air pollution.</p>
<ul>
<li><b>My role:</b> UX researcher and product designer.</li>
<li><b>What I built:</b> A prototype with Khmer and English AQI alerts, health guidance, and an SMS fallback for areas with low internet access.</li>
<li><b>Validation:</b> User interviews and usability testing with Cambodian users.</li>
<li><b>Who it is for:</b> Students, commuters and vulnerable communities.</li>
</ul>
<p><img alt="Product Design" src="https://img.shields.io/badge/Product_Design-D9CCF7?style=flat-square"/> <img alt="Prototype" src="https://img.shields.io/badge/Prototype-D9CCF7?style=flat-square"/></p>
</td>
<td width="33%" valign="top">
<img alt="Innovation" src="https://img.shields.io/badge/Innovation-B8A1E3?style=flat-square"/> <img alt="Top 5 Finalist" src="https://img.shields.io/badge/Top_5_Finalist-E8789F?style=flat-square"/>
<h3>🌧️ Green Flow</h3>
<b>SEA Sponge City Innovation Challenge (2025)</b>
<p>A project addressing urban flooding in Phnom Penh.</p>
<ul>
<li><b>My role:</b> Researcher and technical contributor.</li>
<li><b>What I did:</b> Proposed nature-based flood solutions (rain gardens, bioswales and permeable pathways) and developed the prototype app.</li>
</ul>
<p><img alt="Research" src="https://img.shields.io/badge/Research-D9CCF7?style=flat-square"/> <img alt="Prototype App" src="https://img.shields.io/badge/Prototype_App-D9CCF7?style=flat-square"/></p>
</td>
<td width="33%" valign="top">
<img alt="Innovation" src="https://img.shields.io/badge/Innovation-B8A1E3?style=flat-square"/> <img alt="First Runner-Up" src="https://img.shields.io/badge/First_Runner--Up-E8789F?style=flat-square"/>
<h3>🦻 SDablir</h3>
<b>E-Gen Innovation Program, MoEYS (2025)</b>
<p>An IoT assistive tool for students with disabilities.</p>
<ul>
<li><b>My role:</b> Business analyst and researcher. I represented CamTech in a national competition.</li>
<li><b>What we built:</b> An IoT-based assistive solution for students with disabilities, including hard-of-hearing learners. The Top 5 team was invited to demo the prototype.</li>
</ul>
<p><img alt="IoT" src="https://img.shields.io/badge/IoT-D9CCF7?style=flat-square"/> <img alt="Assistive Tool" src="https://img.shields.io/badge/Assistive_Tool-D9CCF7?style=flat-square"/></p>
</td>
</tr>
</table>

<br/>

<h2 align="center">🌱 Earlier Builds</h2>

<p align="center"><sub>Where I started: HTML, CSS and JavaScript</sub></p>

<table width="100%">
<tr>
<td width="33%" valign="top">
<img alt="Earlier Build" src="https://img.shields.io/badge/Earlier_Build-FFD6E7?style=flat-square"/>
<h3>🌱 Personal Portfolio v1</h3>
<b>First portfolio site</b>
<p>A responsive portfolio site with modern UI components.</p>
<ul>

</ul>
<p><img alt="HTML" src="https://img.shields.io/badge/HTML-D9CCF7?style=flat-square"/> <img alt="CSS" src="https://img.shields.io/badge/CSS-D9CCF7?style=flat-square"/> <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-D9CCF7?style=flat-square"/></p>
<p><a href="https://github.com/SothSokhomal/SothSokhomal_portfolio"><img alt="Source Code" src="https://img.shields.io/badge/Source_Code-E8789F?style=flat-square"/></a></p>
</td>
<td width="33%" valign="top">
<img alt="Earlier Build" src="https://img.shields.io/badge/Earlier_Build-FFD6E7?style=flat-square"/>
<h3>💸 Expense Tracker</h3>
<b>CRUD web app</b>
<p>Add, update and delete daily expense records.</p>
<ul>

</ul>
<p><img alt="HTML" src="https://img.shields.io/badge/HTML-D9CCF7?style=flat-square"/> <img alt="CSS" src="https://img.shields.io/badge/CSS-D9CCF7?style=flat-square"/> <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-D9CCF7?style=flat-square"/></p>
<p><a href="https://github.com/SothSokhomal/expenseapp"><img alt="Source Code" src="https://img.shields.io/badge/Source_Code-E8789F?style=flat-square"/></a></p>
</td>
<td width="33%" valign="top">
<img alt="Earlier Build" src="https://img.shields.io/badge/Earlier_Build-FFD6E7?style=flat-square"/>
<h3>🎵 Spotify UI Clone</h3>
<b>Front-end layout practice</b>
<p>A responsive front-end clone for layout and CSS practice.</p>
<ul>

</ul>
<p><img alt="HTML" src="https://img.shields.io/badge/HTML-D9CCF7?style=flat-square"/> <img alt="CSS" src="https://img.shields.io/badge/CSS-D9CCF7?style=flat-square"/> <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-D9CCF7?style=flat-square"/></p>
<p><a href="https://github.com/SothSokhomal/song_soundie"><img alt="Source Code" src="https://img.shields.io/badge/Source_Code-E8789F?style=flat-square"/></a></p>
</td>
</tr>
</table>

---

## 📜 Certifications

- Scrum Master Certification, Agile Enterprise Coach (2026)
- ASEAN Data Science Explorers, ASEAN Foundation (2026)
- UX/UI Design Short Course, Future.Bit Academy (2025)
- Dynamic Web Development, Champion Coders (2024)

---

<div align="center">

### 💌 Let's connect

I am open to software engineering internships and to collaborating on projects that make technology more accessible.

[Portfolio](https://www.sothsokhomal.com/) · [LinkedIn](https://www.linkedin.com/in/sothvannakrothchansokhomal/) · [Email](mailto:soth.vannakrothchansokhomal@gmail.com)

*Practical software, built with care.* 🌸

</div>
