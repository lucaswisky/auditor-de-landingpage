# Wisky Auditor de Paginas

Sistema de auditoria de landing pages de vendas usando 6 frameworks consagrados de Direct Response.

Analisa qualquer pagina de vendas e gera um relatorio com **scores numericos** e **recomendacoes prioritizadas** para melhorar conversao.

---

## O Que Faz

Voce fornece a URL (ou o conteudo) de uma landing page e o Wisky Auditor analisa com 6 lentes diferentes:

| # | Framework | Fonte | O Que Avalia |
|---|-----------|-------|-------------|
| 1 | **Kennedy 10 Rules** | Dan Kennedy | Compliance com Direct Response |
| 2 | **Message-Market-Media** | Dan Kennedy | Alinhamento mensagem-mercado-midia |
| 3 | **CLOSER** | Alex Hormozi | Jornada do prospect na pagina |
| 4 | **RMBC** | Stefan Georgi | Qualidade da copy (Research, Mechanism, Brief, Copy) |
| 5 | **Value Equation** | Alex Hormozi | Percepcao de valor da oferta |
| 6 | **Design DR** | Best Practices | Elementos visuais e UX |

O resultado e um **score consolidado de 0 a 100** com recomendacoes prioritizadas.

---

## Estrutura do Projeto

```
wisky-auditor-de-paginas/
  squad.yaml                    # Configuracao do squad
  agents/
    wisky-auditor.md            # Agente orquestrador (instrucoes de IA)
  knowledge/
    frameworks-auditoria.md     # Os 6 frameworks detalhados
  tasks/
    auditar-lp.md               # Processo passo a passo
  workflows/
    auditoria-workflow.yaml     # Workflow de execucao
  checklists/
    auditoria-checklist.md      # 15 itens essenciais
  examples/
    exemplo-auditoria.md        # Exemplo de relatorio gerado
```

---

## Como Usar

### Com IA (Claude, ChatGPT, Gemini, etc.)

1. Copie o conteudo de `agents/wisky-auditor.md` e cole como instrucao do sistema (system prompt)
2. Copie o conteudo de `knowledge/frameworks-auditoria.md` como contexto
3. Envie a URL ou conteudo da landing page que quer auditar
4. A IA vai gerar o relatorio completo com scores

### Manual (sem IA)

1. Abra `checklists/auditoria-checklist.md`
2. Abra a landing page que quer auditar
3. Marque cada item do checklist como aprovado ou reprovado
4. Calcule o score: `(itens aprovados / 15) x 100`

---

## Score: Como Interpretar

```
> 90: EXCELENTE -- Pagina otimizada, ajustes finos
80-90: BOM       -- Funciona, mas tem oportunidades
70-80: ADEQUADO  -- Correcoes necessarias antes de escalar trafego
< 70: RUIM       -- Retrabalho significativo necessario
```

---

## Exemplo

Veja um exemplo de relatorio completo em [`examples/exemplo-auditoria.md`](examples/exemplo-auditoria.md).

---

## Licenca

MIT License -- use, modifique e distribua livremente. Veja [LICENSE](LICENSE).

---

Criado por [Lucas Wisky](https://github.com/lucaswisky)
