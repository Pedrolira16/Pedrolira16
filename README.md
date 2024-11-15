<h1 align="center" style="font-size: 28px; font-weight: bold;">Hey 👋, my name is Pedro</h1>
<h3 align="center">Student developer from Brazil</h3>

<br>

- 📚 I’m currently Studying at Cesar School
- 💻 I’m currently learning Javascript

<h3>I have had experience with:</h3>
  <div style="display: inline_block"><br>
    <img align="center" alt="Pedro-Js" height="50" width="60" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
    <img align="center" alt="Pedro-Python" height="50" width="60" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg">
    <img align="center" alt="Pedro-HTML" height="50" width="60" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
    <img align="center" alt="Pedro-Js" height="50" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/c/c-original.svg" /> 
</div>
<br>
<h3>My contacts:</h3>
<div> 
    <a href="https://www.linkedin.com/in/pedro-lira-323598282" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>       
  <a href = "mailto:pedrolira.2004@gmail.com"><img src=https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white></a>
  <a href="https://instagram.com/pedrolir_a" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  
</div>

<h3>These are my stats:</h3>

</div>
 name: Update GitHub Stats

on:
  schedule:
    - cron: "0 */6 * * *"  # Atualiza a cada 6 horas
  workflow_dispatch:       # Permite execução manual do workflow

jobs:
  update-stats:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository content
        uses: actions/checkout@v2

      - name: Run GitHub Stats Updater
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
        run: |
          curl -X GET "https://github-readme-stats.vercel.app/api?username=Pedrolira16&show_icons=true&theme=dark&include_all_commits=true&count_private=true" > README.md
          curl -X GET "https://github-readme-stats.vercel.app/api/top-langs/?username=Pedrolira16&layout=compact&langs_count=7&theme=dark" >> README.md

</div>

