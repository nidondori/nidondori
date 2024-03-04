### Olá 👋

- 🌱 Estudando HTML5 e CSS3
##

<div>
  <a href="https://github.com/nidondori">
    <img height="180em" src="https://github-readme-stats.vercel.app/api?username=nidondori&show_icons=true&theme=cobalt&include_all_commits=true&count_private=true"/>
    <img height="150em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=nidondori&layout=compact&langs_count=16&theme=cobalt"/>
</div>
##
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
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  
<!--
**nidondori/nidondori** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
