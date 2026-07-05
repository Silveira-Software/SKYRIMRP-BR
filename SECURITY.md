# 🔒 Política de Segurança — SKYRIMRP-BR

Levamos a segurança dos jogadores e da infraestrutura a sério. Este documento descreve como reportar vulnerabilidades e como tratamos os reportes.

---

## ⚠️ Reporte vulnerabilidades em PRIVADO

**NÃO** abra issue pública nem publique em Discord/Telegram exploits encontrados.

Em vez disso, envie para:

📧 **seguranca@brlink.site** (assunto: `[SECURITY] resumo curto`)

Ou, se tiver acesso Discord, DM direta ao owner **`@silveira_owner`**.

---

## 📋 O que incluir no reporte

Quanto mais info, mais rápido corrigimos:

- **Tipo de vulnerabilidade** (XSS, SQLi, RCE, auth bypass, etc.)
- **Local afetado** (URL, endpoint, componente).
- **Passos para reproduzir** (sem explorar de fato em produção).
- **Impacto** — o que um atacante consegue fazer.
- **PoC / código** — só se for realmente necessário pra demonstrar.
- **Seu nome / handle** (se quiser crédito público na nota de correção).

---

## ⏱️ O que esperar

| Etapa | Tempo |
|---|---|
| Confirmação de recebimento | até 48h |
| Triagem inicial | até 7 dias |
| Correção em produção | depende da severidade |
| Disclosure coordenado | após patch + nota pública |

### Severidade (CVSS v3.1 simplificado)

- **Crítica (9.0–10.0):** RCE, auth bypass global — patch em horas.
- **Alta (7.0–8.9):** acesso a contas de outros, exfiltração — patch em dias.
- **Média (4.0–6.9):** info disclosure limitada, DoS parcial — patch em semanas.
- **Baixa (0.1–3.9):** UX bugs com impacto de segurança — patch oportunista.

---

## 🏆 Reconhecimento

Reporte válido = crédito público na seção **"Hall da Fama"** abaixo (se você quiser).

> Hall da Fama — *em construção*.

---

## 🚫 O que NÃO fazer

- ❌ Testar exploits em contas de outros jogadores.
- ❌ Acessar/modificar dados que não são seus.
- ❌ Usar vulnerabilidade pra ganho pessoal.
- ❌ Tornar público antes do patch.
- ❌ Vazar dados de outros usuários.

Reportes que violem isso podem ter ação legal — independente da boa-fé.

---

## 🛡️ Práticas nossas (transparência)

- ✅ Senhas com hash bcrypt (nunca plaintext em log).
- ✅ JWT com expiração curta + refresh.
- ✅ HTTPS obrigatório em todos endpoints públicos.
- ✅ Dependências do launcher auditadas (npm audit + verificação manual).
- ✅ Backups diários do banco (retenção 30 dias).
- ✅ Logs de auth com rate limit + alertas de brute force.

---

## 📜 Divulgações anteriores

| Data | Severidade | Descrição | Status |
|---|---|---|---|
| — | — | *nenhuma pública ainda* | — |

---

## 📬 Contato direto

- Email: `seguranca@brlink.site`
- PGP key: *em breve*

Obrigado por ajudar a manter a comunidade segura. 🐉