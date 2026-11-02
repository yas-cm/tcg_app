<div align="center">

<img src="icon-192.png" width="96" alt="Ícone do Side Quest">

# Side Quest

**Contador e diário de partidas de card game.** Por enquanto, de Disney Lorcana.
Registre eventos, partidas e prêmios, e descubra contra quais decks você vai bem ou mal.

Funciona sem internet e fica instalado no celular como um app. · Versão 1.1.1

**[Abrir o app](https://yas-cm.github.io/tcg_app/)**

</div>

<p align="center">
  <img src="screenshots/inicio.png" width="200" alt="Tela inicial com evento em andamento">
  <img src="screenshots/contador.png" width="200" alt="Contador de lore">
  <img src="screenshots/estatisticas.png" width="200" alt="Estatísticas e gráfico de evolução">
  <img src="screenshots/historico.png" width="200" alt="Histórico de eventos por loja">
</p>
<p align="center"><sub>Imagens com dados de exemplo.</sub></p>

## O que ele faz

**Antes de jogar**
- Comece o evento já com tudo preenchido: formato (Core, Selado, Infinity ou Coconut), tipo, nome, local, MD1 ou MD3, rodadas, inscrição e o deck que você vai usar.
- Selados (draft, pré-release, pack rush) sem decklist: coleções, boosters, curva de tinta e as cartas boas que vieram.

**Durante o evento**
- Contador de lore para os dois jogadores, com a metade do oponente virada para o outro lado da mesa.
- Ao chegar a 20 de lore, o resultado do jogo é registrado sozinho. Em MD3, ele já passa para o jogo seguinte.
- Quer só anotar o resultado? Dá para registrar sem usar o contador.
- No fim da partida, é só tocar no deck do oponente. Os decks que você já enfrentou e os seus aparecem como opção, com as cores. Deck novo? Escreva o nome e toque nas cores.
- Etiquetas rápidas e notas para lembrar dos erros e do que mudar no deck.

**Depois**
- Encerramento do evento com colocação e premiação (dinheiro, crédito na loja, boosters e cartas).
- Histórico de eventos separado por loja, com campanha e saldo de cada uma.
- Decks com decklist no formato do duels.ink e histórico do que entrou e saiu.

## Estatísticas

- Taxa de vitória em partidas e em jogos, começando e respondendo.
- Gráfico de evolução (vitórias nas últimas 10 partidas).
- Matchups por cores do oponente, com uma página de notas para cada um.
- Tabela dos seus decks contra os arquétipos que você mais enfrenta.
- Resultado por deck, por tipo de evento e, nos selados, por coleção, com custo por booster e os seus melhores hits.
- Inscrições, prêmios e saldo, separando dinheiro do valor estimado.
- Filtros por deck, período, formato e tipo de evento.
- Exportação em planilha (CSV) e resumo em texto para compartilhar.

## Instalar no celular (Android)

1. Abra o [endereço do app](https://yas-cm.github.io/tcg_app/) no Chrome.
2. Toque no menu ⋮ → **Instalar app** (ou **Adicionar à tela inicial**).
3. Abra uma vez pelo ícone. Depois disso ele funciona sem internet.

## Seus dados

- Tudo fica salvo **só no seu celular**. Nada é enviado para nenhum servidor.
- Faça backup em **Ajustes → Exportar backup** depois de cada evento. No Android, **Compartilhar backup** manda o arquivo direto para o Drive, WhatsApp ou e-mail. O app avisa quando faz mais de 7 dias sem backup.
- Para trocar de celular, use **Ajustes → Importar backup**.

## Como é feito

Um único arquivo HTML, com CSS e JavaScript puros, sem frameworks e sem servidor. Um *service worker* guarda o app para uso offline e os dados ficam no armazenamento do navegador.

| Arquivo | Para que serve |
| --- | --- |
| `index.html` | O app inteiro |
| `sw.js` | Guarda o app para funcionar sem internet |
| `manifest.webmanifest` | Nome, cores e ícones para instalar no celular |
| `icon-*.png` | Ícones do app |

## Versões

- **1.1.1** (02/11/2026): o nome Side Quest aparece ao reinstalar, o app não reabre mais numa partida antiga (o card do início ganhou "Descartar") e o backup pode ser compartilhado.
- **1.1** (02/11/2026): formatos de evento (Core, Selado, Infinity e Coconut), tipo e nome do evento, modo Selado sem decklist (coleções, boosters, curva de tinta e hits), deck do oponente escolhido do mesmo jeito que o seu, MD1 sem "Jogo 1" e tela de novidades.
- **1.0** (28/10/2026): primeira versão. Contador de lore, eventos, registro rápido, decklists, estatísticas, exportação e backup.

## Aviso

Projeto de fã, não oficial, feito para uso pessoal. Disney Lorcana e os símbolos das tintas são marcas e propriedade da Disney e da Ravensburger. Este projeto não é afiliado, patrocinado nem aprovado por elas.
