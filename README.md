# MINAS SEGURAS 3.0
Protótipo acadêmico de transparência ambiental. Site estático responsivo, mapa Leaflet, importação local de CSV público SIGBM/ANM, central de direitos e avaliações locais.

## Publicação
Envie `index.html` e `vercel.json` à raiz do repositório GitHub e importe o repositório na Vercel (Framework: Other; sem build command). Cada commit na branch principal publica nova versão.

## Dados
O site não consulta nem armazena dados de barragens automaticamente. Para visualizar registros, obtenha um CSV oficial pelo SIGBM público ou portal de dados abertos da ANM e importe pelo botão no site. Campos não reconhecidos ficam ausentes. O CSV precisa ter colunas de nome ou município; para marcadores no mapa, latitude e longitude em graus decimais. Se o layout oficial variar, adapte os aliases da função `toRecord`.

## Limitações
O formulário de avaliação utiliza localStorage: cada dispositivo guarda suas próprias respostas, sem coleta centralizada. Não é sistema de emergência, nem oferece atualização em tempo real. Imagens e bibliotecas carregam de servidores externos e exigem internet.
