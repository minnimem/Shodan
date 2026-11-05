# Tabela de Análise (Parte 3 do enunciado)

> Campos marcados com 🔲 dependem de resultado REAL do Shodan.

| Item | Conteúdo |
|---|---|
| 1. Consulta Shodan | `port:27017 country:BR` |
| 2. Identificação do alvo | 🔲 IP `xxx.xxx.xxx.x` / porta 27017 / organização-ASN |
| 3. Evidência do banner | 🔲 Colar trecho literal (ex.: `MongoDB Server Information`) |
| 4. Identificação do serviço | MongoDB — versão 🔲 (se visível) |
| 5. Natureza da exposição | 🔲 Confirmar: ausência de autenticação / configuração padrão insegura |
| 6. OWASP Top 10 | A05:2021 Configuração de Segurança Incorreta (principal); A01:2021 Falha de Controle de Acesso (secundária, só se o banner sustentar) |
| 7. Hipótese de causa raiz | `bind_ip` em `0.0.0.0` sem alteração; ou Docker `-p 27017:27017` sem autenticação; ou security group aberto a `0.0.0.0/0` |
| 8. Correção de menor custo | Vincular a `127.0.0.1`/rede interna; habilitar autenticação (`authorization`); restringir origem no firewall/security group |
