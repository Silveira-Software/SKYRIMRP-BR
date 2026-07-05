# 🗺️ Roadmap público — SKYRIMRP-BR

> Este roadmap mostra **apenas o que podemos divulgar publicamente**. Itens sensíveis (infraestrutura, anti-cheat, exploits conhecidos) ficam internos.

---

## ✅ Já entregue

### Launcher
- Auto-update silencioso do próprio launcher
- Verificação SHA256 dos arquivos do jogo a cada boot
- Login com usuário/senha + JWT
- Detecção automática do Skyrim instalado (Steam)
- Banner de aviso quando o usuário não está logado
- Bloqueio do botão JOGAR sem login válido

### Conta e autenticação
- Cadastro com username/senha
- JWT com expiração de 30 dias
- Hash de senha com bcrypt (custo padrão da indústria)
- Endpoint de validação de token

### Infraestrutura
- Servidor dedicado 24/7 (VPS Linux)
- CDN próprio para distribuição do launcher
- Heartbeat de status a cada 15 segundos
- Página pública de status do servidor (`/server/status`)

### Comunidade
- Discord oficial
- Wiki de regras de RP (em construção)
- Sistema de tickets de suporte

---

## 🚧 Em desenvolvimento (próximas releases)

### Curto prazo (1–2 meses)

- [ ] **Correção de bugs de sessão multiplayer** —investigação em curso.
- [ ] **Whitelist de mods** ampliada (comunidade pediu várias).
- [ ] **Sistema de reports in-game** (`/report jogador motivo`).
- [ ] **Página de changelog público** com notas de cada patch.

### Médio prazo (3–6 meses)

- [ ] **Sistema de clãs/guildas** com tag, chat privado e território.
- [ ] **Economia in-game** — ouro persistido, NPCs comerciantes.
- [ ] **Eventos automáticos** — invasões, festivais, dungeons dinâmicas.
- [ ] **Anti-cheat básico** — detecção de movimento impossível, dup de itens.

### Longo prazo (6+ meses)

- [ ] **Voz in-game** via Mumble (já temos o server, falta integração).
- [ ] **Tradução PT-BR** de diálogos principais (sujeito a aprovação legal).
- [ ] **Mobile companion app** — gerenciar personagem pelo celular.
- [ ] **Sistema de quests custom** — missões criadas pela staff.
- [ ] **Possível expansão pra Oblivion / Fallout 4 MP** se a comunidade quiser.

---

## ❌ Fora de escopo

Pra evitar frustração, listamos o que **NÃO** vamos fazer:

- ❌ Versão standalone / pirata do Skyrim — viola termos da Bethesda.
- ❌ Servidor com P2W (pay-to-win) — o projeto é hobby.
- ❌ Cross-server / multi-realm — exige infra que não temos.
- ❌ Suporte oficial a consoles (PS5/Xbox) — modding é só PC.
- ❌ Mods NSFW ou conteúdo +18 explícito.

---

## 🗳️ Como sugerir novas features

1. Pesquise nas issues abertas se já não foi sugerido.
2. Abra issue com o template `feature-request`.
3. A comunidade vota 👍 / 👎.
4. Staff prioriza mensalmente conforme votos + viabilidade técnica.

---

## 📊 Status atual

**Fase:** Beta fechado
**Jogadores ativos:** informação restrita (só staff)
**Próximo marco:** abertura da whitelist (após correção dos bugs bloqueantes)

---

*Última atualização: julho de 2026 — atualizado mensalmente.*