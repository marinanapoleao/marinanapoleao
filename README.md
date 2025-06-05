<img width=100% src="https://capsule-render.vercel.app/api?type=waving&color=800000&height=120&section=header"/> 

[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=770b1c&size=35&center=true&vCenter=true&width=1000&lines=HELLO!!;Be+Welcome+to+my+profile;My+name+is+Marina+Napoleão;I'm+29+years+old;I'm+from+Brazil;EBAC+Data+Scientist+Student;+:%29)](https://git.io/typing-svg)

Marina Napoleão

 ### Main skills:
 ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)&nbsp; ![SQL](https://img.shields.io/badge/-SQL-0D1117?style=for-the-badge&logo=sql&labelColor=0D1117)&nbsp;

### Contact:
![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)&nbsp;napoleaosmarina@gmail.com

### More information:
📍 Fortaleza/Ceara/Brasil
👩‍🎓 Graduated in Fashion Design
📘 Book lover
🐾 Pet lover

name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: marinanapoleao
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
