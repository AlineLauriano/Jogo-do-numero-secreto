# Descrição
Este projeto consiste em um jogo simples de navegador onde o usuário tenta adivinhar um número secreto gerado aleatoriamente pelo sistema. O jogo é construído com HTML, CSS e JavaScript, e faz uso de uma API de voz para interagir com o usuário.

### Características
O jogo escolhe um número secreto aleatório entre 1 e 10.
O usuário tem tentativas ilimitadas para adivinhar o número.
Após cada tentativa, o jogo informa se o número secreto é maior ou menor que o chute dado.
Quando o usuário acerta o número, o jogo anuncia o sucesso e mostra o número de tentativas utilizadas.
Uma opção para reiniciar o jogo é habilitada após o número secreto ser descoberto.

#### Tecnologias Utilizadas
* HTML5
* CSS3
* JS
* ResponsiveVoice API (para feedback de voz)

### Estrutura do Projeto
O projeto é composto pelos seguintes arquivos:

* index.html: Estrutura principal do jogo, incluindo marcação HTML e links para scripts e folhas de estilo.
* style.css: Folha de estilo para customizar a aparência do jogo.
* app.js: Script que contém a lógica do jogo, manipulação de eventos e interações com a API de voz.

### Como Jogar
1. Abra o arquivo index.html em um navegador compatível.
2. Insira um número entre 1 e 10 no campo de input fornecido.
3. Clique no botão "Chutar" para submeter seu palpite.
4. O jogo irá responder se o número secreto é maior ou menor do que o palpite dado.
5. Continue chutando até acertar o número secreto.
6. Quando o número secreto for descoberto, você pode clicar em "Novo jogo" para reiniciar.

### Funções JavaScript
* gerarNumeroAleatoria(): Gera um número aleatório entre 1 e 10 e garante que o mesmo número não seja escolhido consecutivamente.
* exibirTextoNaTela(tag, texto): Exibe o texto desejado na tag especificada e utiliza a ResponsiveVoice API para ler o texto.
* mensagemInicial(): Exibe a mensagem inicial do jogo.
* verificarChute(): Compara o chute do usuário com o número secreto e fornece feedback adequado.
* limparCampo(): Limpa o campo de input após cada tentativa.
* reiniciarJogo(): Reinicia o jogo, gerando um novo número secreto e resetando o contador de tentativas.
