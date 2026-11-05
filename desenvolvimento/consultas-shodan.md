# Consultas Shodan (conta gratuita)

Estratégia: `count` primeiro → restringir por país/organização → escolher UMA instância.

| Objetivo | Consulta |
|---|---|
| Dimensionar MongoDB no Brasil | `port:27017 country:BR` |
| Reforçar com texto de banner | `"MongoDB Server Information" country:BR` |
| Restringir por organização | `port:27017 country:BR org:"<nome>"` |

**Não usar:** `vuln:` (filtro pago, evitado de propósito).

## Regras
- Apenas leitura do índice; **não** copiar IP para navegador/terminal/ferramenta.
- Anonimizar IP no relatório: `189.xxx.xxx.x`.
- Não discutir como explorar o serviço.
- Registrar a data/hora da consulta.
