### Olá, eu sou Kátia Veloso!!




-  💻Trabalo como Analista de Suporte
- 🌱 Atualmente estou aprendendo Golang, Java e desenvolvimen web
- 👯 I’m looking to collaborate on ..
- 🤔 Embusca de migração para área de programação
- 💬 Ask me about ...
- 📫 Contato e-mail: katisv@gmail.com
- 😄 Pronouns: Ela/Dela


<div style="display: inline_block"><br>
  <img align="center" alt="Rafa-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="center" alt="Rafa-Ts" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-plain.svg">
  <img align="center" alt="Rafa-React" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg">
  <img align="center" alt="Rafa-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="Rafa-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">


<img align="right" alt="Rafa-pic" height="150" style="border-radius:50px;" src="!https://user-images.githubusercontent.com/66650006/229376613-365fa376-c6b6-4c9a-858d-f4b9ba0814d4.gif">
</div>

name: Generate Datas

em :
  cronograma : # executar a cada 12 horas
    - cron : " * */12 * * * "
  workflow_dispatch :

trabalhos :
  construir :
    nome : Jobs para atualizar dados
    run-on : ubuntu-latest
    passos :
      # Animação de Cobra
      - usa : Platane/snk@master
        id : cobra-gif
        com :
          github_user_name : katiasveloso
          svg_out_path : dist/github-contribution-grid-snake.svg

      - usa : crazy-max/ghaction-github-pages@v2.1.3
        com :
          target_branch : saída
          build_dir : dist
        ambiente :
          GITHUB_TOKEN : ${{ segredos.GITHUB_TOKEN }}
