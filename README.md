<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=220&text=Seshan%20Rodrigo&fontSize=55&fontAlignY=40&color=0:0ea5e9,100:9333ea&desc=Aspiring%20AI%20Engineer%20%7C%20Business%20Solutions%20Developer&descAlignY=60&animation=fadeIn" width="100%"/>

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=26&duration=2500&pause=1000&color=38BDF8&center=true&vCenter=true&width=900&lines=AI+%2B+ML+Explorer;Full-Stack+Builder;UI%2FUX+Designer;Future+Tech+Founder;Building+Digital+Business+Solutions" />

<br/><br/>

[![Portfolio](https://img.shields.io/badge/Portfolio-Live_Website-black?style=for-the-badge&logo=vercel&logoColor=white)](https://seshan24.github.io/SeshanPortfolio/)
[![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github)](https://github.com/seshan24)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/seshan-rodrigo-1279ba2b6/)
[![Instagram](https://img.shields.io/badge/Instagram-Follow-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/sesha.n_)

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=seshan24&label=Profile%20Views&color=0e75b6&style=for-the-badge"/>

</div>

---

# 💫 About Me
<img align="right" width="400" src="https://raw.githubusercontent.com/devSouvik/devSouvik/master/gif3.gif"/>

```yaml
Name: Seshan Rodrigo
Role: Aspiring AI Engineer
Education: NIBM x Coventry University
Focus: AI • SaaS • UI/UX • Business Systems
Mission: Build innovative AI-powered business solutions
FunFact: "Call me Sesh 😎"

<p align="center"> <img src="https://skillicons.dev/icons?i=python,php,js,react,nodejs,mongodb,mysql,java,cpp,c,figma,bootstrap,css,git,linux&perline=8"/> </p>

<div align="center"> <img height="180em" src="https://github-readme-stats.vercel.app/api?username=seshan24&show_icons=true&theme=tokyonight&hide_border=true&bg_color=00000000"/> <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=seshan24&layout=compact&theme=tokyonight&hide_border=true&bg_color=00000000"/> <br/> <img width="70%" src="https://github-readme-streak-stats.herokuapp.com/?user=seshan24&theme=tokyonight&hide_border=true&background=00000000"/> </div>

<div align="center">

</div>
<p align="center"> <a href="https://instagram.com/sesha.n_"><img src="https://skillicons.dev/icons?i=instagram" height="55"/></a> <a href="https://www.linkedin.com/in/seshan-rodrigo-1279ba2b6/"><img src="https://skillicons.dev/icons?i=linkedin" height="55"/></a> <a href="https://www.facebook.com/seshan.rodrigo.2025"><img src="https://skillicons.dev/icons?i=facebook" height="55"/></a> </p>

<p align="center"> <a href="https://buymeacoffee.com/seshan"> <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="60"/> </a> </p>

<div align="center">
</div> <img src="https://capsule-render.vercel.app/api?type=waving&color=0:9333ea,100:0ea5e9&height=120&section=footer"/> ```
name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"   # daily
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Generate snake
        uses: Platane/snk@v3
        with:
          github_user_name: seshan24
          outputs: |
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
            dist/github-contribution-grid-snake.svg?palette=github-light

      - name: Push snake animation
        uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
