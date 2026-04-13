✨ Seshan Rodrigo ✨

🚀 AI Engineer in the Making | Full Stack Developer | UI/UX Designer | Business Systems Innovator

------------------------------------------------------------------------

💎 HOLOGRAPHIC PROFILE PANEL

    + Name        : Seshan Rodrigo
    + Role        : Aspiring AI Engineer
    + Focus       : Full Stack + AI + UI/UX + Business Systems
    + Location    : Sri Lanka
    + Current     : Builder.lk Marketplace Platform
    + Mission     : Turning ideas into intelligent digital ecosystems

🧠 AI ENGINEER DNA

    skills:
      frontend: [HTML, CSS, JavaScript, React, UI/UX]
      backend: [PHP, Java, Python, MVC]
      database: [MySQL, Firebase]
      ai: [ML Basics, AI Automation, Smart Systems]
      tools: [Figma, GitHub, VS Code]

🐍 Snake workflow path

.github/workflows/snake.yml

    name: Generate Snake
    on:
      schedule:
        - cron: "0 */12 * * *"
      workflow_dispatch:
    jobs:
      build:
        runs-on: ubuntu-latest
        steps:
          - uses: Platane/snk@v3
            with:
              github_user_name: YOUR_USERNAME
              outputs: dist/snake.svg
