# Governança do Repositório

## Regras básicas

- Proibido commit direto na `main` (tudo entra por PR).
- Branches devem seguir o padrão:
  - `feature/<id>-<resumo>` — novas funcionalidades
  - `fix/<id>-<resumo>` — correção de bugs
  - `chore/<id>-<resumo>` — tarefas de manutenção/configuração

## DoD do PR (mínimo)

- **Descrição**: o que mudou, por quê e como testar.
- **Auto-review**: checklist preenchido + mínimo de 3 comentários técnicos no diff do PR,
  usando os rótulos `[Risco]`, `[Manutenção]` ou `[Teste]`.
- Nenhuma discussão aberta pode ficar pendente no momento do merge.

## Review (critérios)

- Comentários devem explicar o motivo e sugerir alternativa quando possível.
- Evitar "é opinião minha" sem embasamento; toda sugestão precisa de justificativa técnica.
- Evitar PR grande: se não dá para revisar em ~10 min, dividir em PRs menores.

## Proteção da branch `main`

- Merge só é permitido via Pull Request aprovado.
- Push direto na `main` é bloqueado por regra de proteção no repositório remoto.
- Conversas abertas devem ser resolvidas antes do merge (Require conversation resolution).
