# cinek-posts

Mídias dos posts do Instagram do CineK (curiosidades de cinema). Os arquivos daqui são públicos, porque o Instagram baixa os vídeos por link na hora de publicar.

Regra do perfil: nenhum post fala do app CineK.

## Fila de publicação (automática)

- `fila.json` guarda os itens e o status de cada um: `pendente`, `publicado`, `pausado` ou `erro`.
- `publicar.py` publica o próximo item `pendente`. É a mesma lógica do eletrik-posts.
- Antes de ligar, preencha `IG_USER` no `publicar.py` com o ID da conta do Instagram do CineK.
- **Para adicionar um vídeo:** só depois que o Klaus aprovar, faça push de uma pasta `videos/NN-slug/` com `video.mp4` e `legenda.txt`. Ela entra na fila sozinha, na ordem do nome da pasta.
- **Para segurar um item:** mude o status dele para `pausado` no `fila.json`.
