# Reconhecimento de Superfície de Exposição com Shodan e Análise de Causa Raiz

**Instituição:** Centro Universitário de Goiás – UniGoiás
**Disciplina:** Segurança da Informação — Prof. Tiago Marcelino Reis
**Aluno:** Diego de Jesus Modesto Silva
**Ano:** 2026

## Sobre
Atividade em sala (150 min) de análise **passiva** de serviços expostos na internet usando o índice do Shodan, com atribuição a uma categoria do OWASP Top 10 (2021), hipótese de causa raiz e correção de menor custo.

Serviço analisado: **MongoDB (`port:27017`)**.

> ⚠️ **Premissa ética:** somente dados do índice passivo do Shodan. Nenhuma conexão, login, varredura ou exploração. IPs anonimizados (último octeto → `x`).

## Estrutura
```
.
├── trabalho/        # Entrega final (.docx)
├── enunciado/       # PDF original da atividade
└── desenvolvimento/ # Material de desenvolvimento
    ├── consultas-shodan.md       # Consultas gratuitas e estratégia de busca
    ├── tabela-analise.md         # Tabela de 8 itens (a preencher com dados reais)
    ├── checklist-entrega.md      # Checklist de requisitos e avaliação
    └── evidencias/               # Capturas de tela (com IP mascarado)
```

## Pendências antes da entrega
Ver [`desenvolvimento/checklist-entrega.md`](desenvolvimento/checklist-entrega.md). O principal: preencher o banner **real** do Shodan; ele não pode ser inventado.
