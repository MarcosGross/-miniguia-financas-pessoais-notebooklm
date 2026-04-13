# 📚 miniguia-financas-pessoais-notebooklm

> Caderno temático criado com o auxílio do **Google NotebookLM** como parte do desafio prático da DIO.  
> Tema escolhido: **Finanças Pessoais para Iniciantes**

![Status](https://img.shields.io/badge/status-concluído-brightgreen)
![Tema](https://img.shields.io/badge/tema-finanças%20pessoais-blue)
![Ferramenta](https://img.shields.io/badge/ferramenta-NotebookLM-orange)
![DIO](https://img.shields.io/badge/plataforma-DIO-purple)

---

## 📋 Sumário

1. [Contexto e Objetivos](#1-contexto-e-objetivos)
2. [Curadoria de Fontes](#2-curadoria-de-fontes)
3. [Engenharia de Prompts e Cicatrizes](#3-engenharia-de-prompts-e-cicatrizes)
4. [Miniguia de Estudo — Entrega Final](#4-miniguia-de-estudo--entrega-final)
   - [Resumos Estruturados](#41-resumos-estruturados)
   - [Glossário de Conceitos](#42-glossário-de-conceitos)
   - [Prompts Reutilizáveis](#43-prompts-reutilizáveis)

---

## 1. Contexto e Objetivos

### Por que Finanças Pessoais?

A educação financeira ainda é um tema pouco explorado na formação básica brasileira. Segundo a ANBIMA, apenas **29% dos brasileiros** têm algum tipo de investimento, e a maioria nunca aprendeu formalmente sobre orçamento, dívidas ou poupança. Escolhi esse tema por ser **universalmente aplicável**, com vasta literatura aberta disponível e impacto direto na qualidade de vida.

### Objetivos de Estudo

Ao final deste caderno temático, o objetivo é ser capaz de:

- [ ] Compreender o conceito de **orçamento pessoal** e como montá-lo na prática
- [ ] Diferenciar **ativos** de **passivos** na perspectiva do investidor individual
- [ ] Entender o funcionamento básico de **juros compostos** e seu impacto no longo prazo
- [ ] Conhecer as principais **modalidades de investimento** acessíveis ao iniciante (Tesouro Direto, CDB, fundos)
- [ ] Aplicar a regra **50/30/20** como ponto de partida para organização financeira
- [ ] Usar o NotebookLM como ferramenta de síntese e revisão ativa

---

## 2. Curadoria de Fontes

As fontes foram selecionadas com base em três critérios: **acesso aberto**, **confiabilidade institucional** e **linguagem acessível ao iniciante**.

| # | Título | Fonte | Formato | Link |
|---|--------|--------|---------|------|
| 1 | Caderno de Educação Financeira — Gestão de Finanças Pessoais | Banco Central do Brasil (BCB) | PDF | [🔗 Acessar](https://www.bcb.gov.br/content/cidadaniafinanceira/Documents/publicacoes/serie_cidadania/Fasciculo_Gestao_Financas_Pessoais.pdf) |
| 2 | Guia de Educação Financeira | ENEF / Estratégia Nacional de Educação Financeira | PDF | [🔗 Acessar](https://www.vidaedinheiro.gov.br/wp-content/uploads/2017/08/Guia-de-Educacao-Financeira.pdf) |
| 3 | Como se Planejar Financeiramente | Tesouro Nacional | PDF | [🔗 Acessar](https://www.tesourodireto.com.br/data/files/20/01/23/42/A5E9F610EEFCCA57B8C80EA8/Cartilha_Planejamento_Financeiro.pdf) |
| 4 | Série Cidadania Financeira — Investimentos e Mercado Financeiro | Banco Central do Brasil (BCB) | PDF | [🔗 Acessar](https://www.bcb.gov.br/content/cidadaniafinanceira/Documents/publicacoes/serie_cidadania/Fascículo%206%20-%20Investimentos%20e%20Mercado%20Financeiro.pdf) |
| 5 | Caderneta de Poupança e Alternativas de Investimento (CVM Educacional) | CVM — Comissão de Valores Mobiliários | HTML/PDF | [🔗 Acessar](https://www.investidor.gov.br/menu/Menu_Investidor/a_investimentos/Caderneta_Poupanca.html) |

> **Nota de curadoria:** Todas as fontes são de órgãos reguladores ou do governo federal, o que garante isenção e precisão técnica. Os PDFs foram carregados diretamente no NotebookLM para que a IA pudesse cruzar informações entre eles.

---

## 3. Engenharia de Prompts e Cicatrizes

Esta seção documenta o processo real de interação com o NotebookLM: as perguntas feitas, as variações testadas, os resultados obtidos e as dificuldades encontradas (as "cicatrizes").

---

### 3.1 Rodada 1 — Entendendo o Orçamento Pessoal

#### Prompt inicial (muito genérico)
```
O que é orçamento pessoal?
```
**Problema:** A resposta foi correta, mas superficial. O NotebookLM resumiu o conceito sem referenciar as fontes específicas.

#### Prompt refinado
```
Com base nos documentos carregados, explique o conceito de orçamento pessoal 
e quais etapas práticas o Banco Central recomenda para montá-lo.
```
**Resultado:** Muito melhor. A IA citou diretamente o Fasciculo do BCB, mencionando as etapas de: (1) levantamento de receitas, (2) mapeamento de despesas fixas e variáveis, (3) identificação do saldo e (4) definição de metas.

**Referência gerada pelo NotebookLM:** Fascículo — Gestão de Finanças Pessoais (BCB), p. 12-18.

#### 🩹 Cicatriz registrada
> Prompts genéricos sem ancoragem nas fontes geram respostas genéricas. Sempre indicar explicitamente "com base nos documentos" ou mencionar a fonte específica desejada.

---

### 3.2 Rodada 2 — Juros Compostos

#### Prompt testado (versão 1)
```
Explique juros compostos.
```
**Problema:** Resposta didática, mas sem exemplos numéricos práticos e sem vínculo com as fontes.

#### Prompt testado (versão 2)
```
Explique juros compostos como se eu tivesse 20 anos e nunca tivesse 
investido nada. Use um exemplo com valores em reais e mencione o que 
os documentos dizem sobre o tempo como fator de crescimento.
```
**Resultado:** A IA criou um exemplo com R$ 200/mês investidos por 10, 20 e 30 anos a 0,8% a.m., conectando ao conceito de "tempo como aliado" presente no Guia da ENEF.

**Referência gerada:** Guia de Educação Financeira (ENEF), Capítulo 3 — Poupança e Investimento.

#### Prompt testado (versão 3 — comparativo)
```
Compare o efeito dos juros compostos em: (a) uma dívida no cartão de crédito 
e (b) um investimento em Tesouro Selic, usando os dados das fontes disponíveis.
```
**Resultado:** Excelente. A IA usou as duas perspectivas (dívida vs. investimento), cruzando informações do BCB e da CVM, tornando o conceito muito mais concreto.

#### 🩹 Cicatriz registrada
> Pedir comparativos ou analogias ("como se tivesse X anos", "compare A e B") aumenta significativamente a qualidade e a ancoragem nas fontes.

---

### 3.3 Rodada 3 — Tipos de Investimento

#### Prompt testado (versão 1)
```
Quais são os investimentos para iniciantes?
```
**Problema:** Lista genérica sem critérios de comparação e sem mencionar risco ou liquidez.

#### Prompt refinado
```
Com base nos documentos da CVM e do Banco Central, liste os principais 
investimentos recomendados para quem está começando, comparando: 
rentabilidade esperada, liquidez e nível de risco. Organize em formato de tabela.
```
**Resultado:** Tabela clara com Poupança, CDB, Tesouro Direto (Selic e IPCA+) e Fundos de Renda Fixa, com referências precisas às páginas dos documentos.

#### Prompt adicional testado
```
Por que o Tesouro Selic é considerado mais seguro que a poupança, 
segundo os documentos do Tesouro Nacional e do BCB?
```
**Resultado:** A IA explicou a garantia do FGC (Fundo Garantidor de Créditos), a cobertura do Tesouro Nacional e as diferenças de rentabilidade. Resposta com boa profundidade técnica.

#### 🩹 Cicatriz registrada
> Pedir estruturas específicas de saída ("organize em tabela", "liste em tópicos", "responda em 3 parágrafos") melhora muito a usabilidade da resposta para estudo.

---

### 3.4 Rodada 4 — Síntese e Revisão

#### Prompt de síntese
```
Gere um resumo executivo de no máximo 300 palavras sobre os três 
pilares da saúde financeira pessoal, segundo os documentos carregados.
```
**Resultado:** Resumo coeso, com os pilares: (1) controle de gastos/orçamento, (2) eliminação de dívidas, (3) construção de reserva e investimento. Referências distribuídas entre BCB, ENEF e Tesouro Nacional.

#### Prompt de quiz para revisão
```
Com base nos documentos, crie 5 perguntas de múltipla escolha sobre 
finanças pessoais para iniciantes, com gabarito comentado.
```
**Resultado:** Quiz funcional e bem embasado. Excelente para revisão ativa.

#### 🩹 Cicatriz registrada
> O NotebookLM tende a "não inventar" quando as fontes são sólidas — mas pode omitir detalhes se o tema não estiver bem coberto nos PDFs. Quando isso acontecer, adicionar uma fonte complementar resolve.

---

### Tabela-Resumo da Engenharia de Prompts

| Padrão | Estratégia | Resultado |
|--------|-----------|-----------|
| ❌ Genérico | "Explique X" | Superficial, sem âncora nas fontes |
| ✅ Ancorado | "Com base nos documentos, explique X" | Preciso, com referências |
| ✅ Persona | "Explique como se eu tivesse 20 anos" | Linguagem acessível e contextualizada |
| ✅ Comparativo | "Compare A e B segundo os documentos" | Resposta densa e com cruzamento de fontes |
| ✅ Estruturado | "Organize em tabela / liste em tópicos" | Saída pronta para uso e revisão |
| ✅ Síntese | "Resumo de X palavras sobre Y" | Ótimo para consolidar aprendizado |
| ✅ Quiz | "Crie 5 perguntas com gabarito" | Excelente para revisão ativa |

---

## 4. Miniguia de Estudo — Entrega Final

---

### 4.1 Resumos Estruturados

#### 📌 Bloco 1: Orçamento Pessoal

O orçamento pessoal é o mapeamento de todas as entradas (receitas) e saídas (despesas) de dinheiro em um período. O Banco Central recomenda quatro etapas:

1. **Levantar todas as receitas** — salário, freela, renda extra
2. **Mapear despesas fixas** — aluguel, parcelas, mensalidades
3. **Mapear despesas variáveis** — alimentação, lazer, transporte
4. **Calcular o saldo** — o que sobra (ou falta) ao final do mês

A **Regra 50/30/20** é um ponto de partida prático:
- **50%** para necessidades (moradia, alimentação, transporte)
- **30%** para desejos (lazer, assinaturas, restaurantes)
- **20%** para poupança e investimentos

---

#### 📌 Bloco 2: Dívidas e Juros

Dívidas não são necessariamente ruins — o problema está nos **juros abusivos**. No Brasil, as modalidades com maiores taxas são:

| Modalidade | Taxa média anual (ref. BCB) |
|------------|----------------------------|
| Cartão de crédito rotativo | ~430% a.a. |
| Cheque especial | ~130% a.a. |
| Crédito pessoal (fintech) | ~60–90% a.a. |
| Crédito consignado | ~20–35% a.a. |

**Estratégia recomendada:** quitar as dívidas de maior taxa primeiro (método avalanche) antes de investir.

---

#### 📌 Bloco 3: Juros Compostos e o Poder do Tempo

Juros compostos são calculados sobre o montante acumulado, não apenas sobre o valor inicial. A fórmula é:

```
M = C × (1 + i)^t

Onde:
M = montante final
C = capital inicial
i = taxa de juros por período
t = número de períodos
```

**Exemplo prático:**

| Investimento mensal | Taxa | 10 anos | 20 anos | 30 anos |
|--------------------|------|---------|---------|---------|
| R$ 200 | 0,8% a.m. | R$ 36.833 | R$ 119.427 | R$ 299.017 |
| R$ 500 | 0,8% a.m. | R$ 92.082 | R$ 298.568 | R$ 747.543 |

> Conclusão: **começar cedo importa mais do que o valor aplicado.**

---

#### 📌 Bloco 4: Principais Investimentos para Iniciantes

| Investimento | Rentabilidade | Liquidez | Risco | Ideal para |
|-------------|--------------|---------|-------|------------|
| Poupança | ~70% da Selic | Alta (D+0) | Baixíssimo | Reserva de emergência (curto prazo) |
| Tesouro Selic | ~100% da Selic | Alta (D+1) | Baixíssimo | Reserva de emergência / curto prazo |
| CDB (grandes bancos) | 90-100% CDI | Média/Alta | Baixo (FGC) | Médio prazo |
| CDB (fintechs) | 110-130% CDI | Média | Baixo (FGC) | Médio prazo |
| Tesouro IPCA+ | IPCA + 5-7% a.a. | Média (D+1) | Baixo | Longo prazo / aposentadoria |
| Fundos de Renda Fixa | Variável | Média | Baixo-médio | Diversificação simples |

> **FGC** (Fundo Garantidor de Créditos): garante até R$ 250.000 por CPF por instituição em produtos bancários (CDB, poupança, LCI, LCA).

---

#### 📌 Bloco 5: Reserva de Emergência

Antes de investir para crescer patrimônio, é fundamental construir uma **reserva de emergência**:

- **Valor ideal:** de 3 a 6 meses das despesas mensais
- **Onde manter:** Tesouro Selic ou CDB com liquidez diária
- **Por que não a poupança:** o Tesouro Selic rende mais com liquidez equivalente

---

### 4.2 Glossário de Conceitos

| Termo | Definição |
|-------|-----------|
| **Ativo** | Bem ou direito que gera renda ou pode ser convertido em dinheiro (imóvel alugado, investimento) |
| **Passivo** | Obrigação financeira que consome renda (dívida, parcela, financiamento) |
| **CDI** | Certificado de Depósito Interbancário — taxa de referência para investimentos de renda fixa no Brasil, próxima à Selic |
| **Selic** | Taxa básica de juros da economia brasileira, definida pelo COPOM (Comitê de Política Monetária) |
| **IPCA** | Índice Nacional de Preços ao Consumidor Amplo — principal índice de inflação brasileiro |
| **FGC** | Fundo Garantidor de Créditos — seguro que protege até R$ 250 mil por CPF por instituição em produtos bancários |
| **Liquidez** | Facilidade e velocidade com que um investimento pode ser convertido em dinheiro sem perda de valor |
| **Rentabilidade** | Retorno financeiro gerado por um investimento em determinado período |
| **Juros compostos** | Juros calculados sobre o saldo acumulado, incluindo juros anteriores ("juros sobre juros") |
| **Juros simples** | Juros calculados apenas sobre o capital inicial |
| **Tesouro Direto** | Programa do governo federal que permite a pessoas físicas comprarem títulos públicos pela internet |
| **CDB** | Certificado de Depósito Bancário — título emitido por bancos para captar recursos; rendimento geralmente atrelado ao CDI |
| **Renda fixa** | Classe de investimento cujas regras de rendimento são conhecidas no momento da aplicação |
| **Renda variável** | Classe de investimento cujo retorno não é previsível (ações, FIIs, ETFs) |
| **Diversificação** | Estratégia de distribuir investimentos em diferentes ativos para reduzir risco |
| **Orçamento pessoal** | Controle estruturado de receitas e despesas para alcançar metas financeiras |
| **Reserva de emergência** | Valor guardado em investimentos de alta liquidez para cobrir imprevistos |
| **Regra 50/30/20** | Método de alocação de renda: 50% necessidades, 30% desejos, 20% poupança/investimento |
| **COPOM** | Comitê de Política Monetária — órgão do Banco Central responsável por definir a taxa Selic |
| **Patrimônio líquido** | Diferença entre o total de ativos e o total de passivos de uma pessoa |

---

### 4.3 Prompts Reutilizáveis

Use os prompts abaixo em futuras sessões no NotebookLM (ou em qualquer LLM) para revisão e aprofundamento do tema.

---

#### 🔁 Prompts de Revisão Conceitual

```
Com base nos documentos carregados, explique [CONCEITO] de forma simples, 
usando um exemplo prático com valores em reais.
```

```
Quais são as principais diferenças entre [CONCEITO A] e [CONCEITO B] 
segundo os documentos? Organize em uma tabela comparativa.
```

```
Resuma em até 5 tópicos o que os documentos dizem sobre [TEMA].
```

---

#### 🔁 Prompts de Aplicação Prática

```
Tenho [VALOR] por mês para investir e um horizonte de [TEMPO]. 
Com base nos documentos, quais seriam os passos recomendados para começar?
```

```
Crie um exemplo de orçamento mensal para uma pessoa com renda de R$ [VALOR], 
aplicando a Regra 50/30/20 conforme descrito nos documentos.
```

```
Simule o crescimento de uma aplicação de R$ [VALOR] por mês 
durante [ANOS] anos com taxa de [TAXA]% ao mês, explicando o papel 
dos juros compostos nesse resultado.
```

---

#### 🔁 Prompts de Quiz e Revisão Ativa

```
Crie 5 perguntas de múltipla escolha sobre [TEMA] com base nos documentos. 
Inclua o gabarito comentado ao final.
```

```
Qual seria a pergunta mais importante que um iniciante em finanças 
deveria fazer sobre [TEMA]? Responda com base nos documentos.
```

```
Cite 3 erros comuns que os documentos mencionam em relação a [TEMA] 
e como evitá-los.
```

---

#### 🔁 Prompts de Síntese e Consolidação

```
Gere um resumo executivo de no máximo 200 palavras sobre [TEMA], 
com base nos documentos carregados. Use linguagem simples.
```

```
Monte um plano de estudo de 4 semanas sobre finanças pessoais com base 
nos documentos, indicando quais tópicos priorizar em cada semana.
```

```
Quais são os 3 conceitos mais importantes que alguém precisa dominar 
antes de começar a investir, segundo os documentos? Explique cada um.
```

---

#### 🔁 Prompts de Troubleshooting (quando a IA não responde bem)

```
Sua resposta anterior foi muito genérica. Por favor, referencie 
explicitamente qual documento e qual trecho embasa cada afirmação.
```

```
Adicione um exemplo numérico prático à sua explicação anterior sobre [TEMA].
```

```
Reformule a resposta anterior em formato de tabela comparativa, 
incluindo as colunas: [coluna1], [coluna2], [coluna3].
```

---

## 🧾 Considerações Finais

Este caderno demonstrou que o **NotebookLM é uma ferramenta poderosa para aprendizagem ativa** — especialmente quando se é investido tempo na engenharia de prompts. Os principais aprendizados do processo foram:

1. **Qualidade das fontes determina qualidade das respostas** — fontes técnicas e confiáveis geram sínteses mais precisas
2. **Prompts ancorados nas fontes são sempre superiores** a perguntas genéricas
3. **Pedir estruturas de saída específicas** (tabela, tópicos, quiz) aumenta muito a utilidade pedagógica das respostas
4. **Registrar as "cicatrizes"** (o que não funcionou e por quê) é tão valioso quanto registrar o que funcionou

---

## 📎 Referências Completas

1. BANCO CENTRAL DO BRASIL. *Série Cidadania Financeira: Gestão de Finanças Pessoais*. Brasília: BCB, 2013. Disponível em: https://www.bcb.gov.br
2. ENEF — ESTRATÉGIA NACIONAL DE EDUCAÇÃO FINANCEIRA. *Guia de Educação Financeira*. Brasília: ENEF, 2017. Disponível em: https://www.vidaedinheiro.gov.br
3. TESOURO NACIONAL. *Cartilha de Planejamento Financeiro*. Brasília: STN, 2022. Disponível em: https://www.tesourodireto.com.br
4. BANCO CENTRAL DO BRASIL. *Série Cidadania Financeira: Investimentos e Mercado Financeiro*. Brasília: BCB, 2014. Disponível em: https://www.bcb.gov.br
5. CVM — COMISSÃO DE VALORES MOBILIÁRIOS. *Portal do Investidor: Caderneta de Poupança e Alternativas*. Rio de Janeiro: CVM, 2023. Disponível em: https://www.investidor.gov.br

---

