# Sorteio de Times — Pelada de Quarta e Sábado

App web para organizar o sorteio de times da pelada, separando quem chega no horário de quem chega atrasado — sem depender de papel e caneta na beira do campo.

**App no ar:** https://sorteio-times-pelada-verakt.vercel.app

## O que o app faz

1. **Colar confirmados** — cole a lista de confirmação como ela sai do WhatsApp (com numeração, ✅/❌ na frente, emojis, tags como "PG"). O app limpa tudo sozinho:
   - Remove numeração, emojis e a tag "PG".
   - Ignora automaticamente quem está na lista de "Fora" (linhas com ❌).
   - Ignora cabeçalhos, avisos e informações de Pix que não sejam nomes numerados.
2. **Lista de confirmados** — cada jogador aparece como um "chip" que pode ser marcado como **No horário** ou **Atrasado**, e removido se necessário. Também dá para adicionar alguém manualmente (ex: um atrasado que não estava na lista original).
3. **Sortear** — define quantos jogadores por time (varia toda semana) e sorteia aleatoriamente só com quem está marcado como "no horário". Os times são preenchidos cheios em sequência; se sobrar gente, vira **um único time menor no final** (em vez de espalhar a sobra em vários times incompletos).
4. **Distribuir atrasados** — depois do sorteio, um botão separado distribui quem chegou atrasado, um por um, sempre no(s) time(s) com menos jogadores no momento — sem precisar resortear quem já está jogando.

## Detalhes técnicos

- Arquivo único (`index.html`), sem dependências externas além das fontes do Google Fonts.
- Sorteio 100% aleatório (sem considerar nível técnico dos jogadores).
- Nenhum dado é salvo entre sessões — cada dia de jogo você cola a lista de novo.
- Hospedado na Vercel.

## Como atualizar

O código-fonte completo está em `index.html`. Para publicar uma alteração, é só reenviar o arquivo atualizado para o mesmo projeto na Vercel (mesmo link, mesmo alias).

## Ideias para o futuro

- Salvar um grupo de jogadores fixos (roster recorrente), para não precisar colar a lista inteira toda semana — só ajustar quem faltou ou chegou atrasado.
