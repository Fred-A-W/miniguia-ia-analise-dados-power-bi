# 📘 Miniguia de Estudos

## Inteligência Artificial Generativa aplicada à Análise de Dados com Power BI e DAX

Este miniguia reúne os principais conhecimentos consolidados durante o desenvolvimento do Caderno Temático no NotebookLM.

O material foi construído a partir das cinco fontes oficiais selecionadas, dos experimentos realizados com diferentes prompts e da análise crítica das respostas produzidas pela Inteligência Artificial.

---

# 🎯 Objetivo do Miniguia

Consolidar os conhecimentos adquiridos sobre:

* Inteligência Artificial Generativa;
* Engenharia de Prompts;
* Microsoft Power BI;
* Copilot no Power BI;
* linguagem DAX;
* aplicações práticas da IA na análise de dados;
* limitações e cuidados na utilização de IA.

O objetivo não é apenas memorizar conceitos, mas compreender como esses conhecimentos podem ser utilizados de forma prática e crítica.

---

# 1. 🤖 Inteligência Artificial Generativa

## O que é?

A Inteligência Artificial Generativa é uma área da Inteligência Artificial capaz de gerar novos conteúdos a partir de instruções fornecidas pelo usuário.

Entre os conteúdos que podem ser gerados estão:

* textos;
* imagens;
* áudio;
* vídeo;
* código.

A tecnologia utiliza modelos de aprendizado profundo e redes neurais treinadas com grandes volumes de dados.

## Conceitos importantes

### Deep Learning

Técnica de aprendizado de máquina baseada em redes neurais profundas, utilizada para identificar padrões em grandes volumes de dados.

### Modelos de base

Modelos treinados com grandes conjuntos de dados que podem ser utilizados como base para diferentes tarefas e aplicações.

### Transformers

Arquitetura utilizada por muitos modelos modernos de IA, baseada em mecanismos de atenção para compreender relações entre diferentes partes de uma sequência.

### Atenção

Mecanismo que permite ao modelo considerar diferentes partes de uma sequência ao processar uma informação.

### Fine-tuning

Processo de adaptação de um modelo previamente treinado para uma tarefa ou contexto específico.

### RAG

Retrieval-Augmented Generation é uma abordagem que permite complementar a geração de respostas utilizando informações recuperadas de fontes externas ao conjunto original de treinamento.

## Principal aprendizado

A IA Generativa possui grande capacidade de produzir conteúdo, mas suas respostas precisam ser analisadas criticamente.

---

# 2. 🧠 Engenharia de Prompts

## O que é?

Engenharia de Prompts é o processo de elaborar e aprimorar instruções fornecidas a modelos de Inteligência Artificial para orientar as respostas de acordo com determinado objetivo.

Um prompt bem estruturado pode combinar:

**Papel + Contexto + Objetivo + Restrições + Formato de saída**

## Características de um bom prompt

### Clareza

O pedido deve ser compreensível e evitar ambiguidades.

### Contexto

Informações relevantes devem ser fornecidas para ajudar a IA a interpretar corretamente a tarefa.

### Especificidade

Quanto mais claro for o objetivo, maior tende a ser o controle sobre a resposta.

### Restrições

Podem ser utilizadas para delimitar o que deve ou não aparecer na resposta.

### Formato

É possível especificar como a resposta deverá ser apresentada, por exemplo:

* tabela;
* lista;
* resumo;
* passo a passo;
* código.

---

## Principais técnicas estudadas

### Zero-shot

A IA recebe a solicitação sem exemplos prévios.

**Exemplo:**

> Explique o que é DAX.

### One-shot

Um exemplo é fornecido para orientar o formato ou padrão da resposta.

### Few-shot

São fornecidos alguns exemplos para orientar o comportamento desejado.

### Chain of Thought

Estratégia apresentada nas fontes para decomposição de tarefas e problemas mais complexos em etapas.

## Principal aprendizado

A Engenharia de Prompts não consiste apenas em elaborar perguntas mais longas.

O mais importante é fornecer **informação suficiente, contexto adequado e um objetivo claramente definido**.

---

# 3. 📊 Microsoft Power BI

## O que é?

O Power BI é uma plataforma utilizada para preparação, modelagem, análise e visualização de dados.

Entre seus principais componentes estão:

* Power BI Desktop;
* Power BI Service;
* modelos semânticos;
* relatórios;
* dashboards;
* workspaces;
* gateways.

## Modelo semântico

O modelo semântico organiza os dados e seus relacionamentos para utilização em análises e relatórios.

Uma boa preparação do modelo é importante para o uso de recursos de Inteligência Artificial, inclusive o Copilot.

## Modelagem

Entre as boas práticas estudadas está a utilização do **esquema estrela**, com organização entre tabelas de fatos e dimensões.

## Principal aprendizado

A Inteligência Artificial não substitui uma boa modelagem de dados.

A organização, a qualidade e o contexto dos dados são fundamentais para obter análises adequadas.

---

# 4. 🤖 Copilot no Power BI

## O que é?

O Copilot é um recurso de Inteligência Artificial integrado ao Power BI para apoiar usuários em determinadas tarefas relacionadas à análise e produção de conteúdo.

## Possibilidades estudadas

Entre as aplicações documentadas estão:

* geração de expressões DAX;
* escrita de consultas DAX;
* refinamento de medidas;
* criação de descrições para medidas;
* geração de resumos;
* apoio à criação e compreensão de relatórios;
* interação com dados.

## Preparação dos dados

Um dos principais aprendizados do projeto foi a importância de preparar adequadamente o modelo semântico.

Dados e modelos mal estruturados podem dificultar a interpretação do contexto e contribuir para respostas genéricas, imprecisas ou inadequadas.

## Cuidados

O uso do Copilot deve considerar:

* configuração do ambiente;
* requisitos de capacidade e licenciamento;
* limites técnicos;
* qualidade do modelo semântico;
* necessidade de validação humana.

> Recursos, requisitos e limites de produtos podem ser atualizados. Antes de uma implementação real, recomenda-se consultar a documentação oficial mais recente da Microsoft.

---

# 5. 🧮 DAX

## O que é?

**DAX — Data Analysis Expressions** é uma linguagem de expressões utilizada para realizar cálculos e consultas em modelos de dados tabulares.

No Power BI, DAX pode ser utilizada para criar diferentes tipos de objetos.

---

## Medidas

Medidas são cálculos avaliados dinamicamente de acordo com o contexto em que são utilizados.

### Exemplo

```DAX
Total Vendas = SUM('Sales'[SalesAmount])
```

A medida acima calcula a soma dos valores existentes na coluna `SalesAmount` da tabela `Sales`.

---

## Colunas calculadas

São colunas criadas por meio de expressões DAX e avaliadas para as linhas da tabela.

---

## Tabelas calculadas

São tabelas criadas utilizando expressões DAX.

---

## RLS

**Row-Level Security** ou Segurança em Nível de Linha é utilizada para controlar quais registros podem ser visualizados de acordo com regras e funções definidas.

---

# 6. 🧩 Contexto no DAX

O conceito de contexto é fundamental para compreender o comportamento dos cálculos DAX.

## Contexto de linha

Refere-se à linha atualmente avaliada por uma expressão.

## Contexto de filtro

Representa as restrições aplicadas aos dados por filtros, segmentações ou outras condições.

## Contexto de consulta

Está relacionado ao conjunto de informações solicitado por uma consulta ou visual.

## Principal aprendizado

Compreender o contexto é essencial para interpretar corretamente os resultados das medidas e identificar possíveis problemas em cálculos DAX.

---

# 7. 🤝 Inteligência Artificial aplicada ao DAX

A Inteligência Artificial Generativa pode apoiar o profissional de dados em tarefas como:

* criação de rascunhos de medidas;
* geração de consultas DAX;
* refinamento de medidas;
* documentação;
* explicação de fórmulas;
* organização da lógica de cálculos;
* identificação de possíveis problemas.

## Exemplo

Uma solicitação simples:

```text
Crie uma medida DAX para calcular o total de vendas.
```

Pode ser melhorada com contexto:

```text
Atue como especialista em Power BI e DAX.

Tenho uma tabela chamada Sales e uma coluna numérica chamada SalesAmount.

Crie uma medida chamada Total Vendas para calcular a soma
dos valores de SalesAmount.

Apresente o código DAX, explique seu funcionamento
e indique quais pontos devem ser validados antes do uso.
```

## Principal aprendizado

A IA pode acelerar o trabalho, mas o profissional continua responsável por validar o código e os resultados.

---

# 8. ⚠️ Limitações e cuidados

## Alucinações

A IA pode produzir informações incorretas ou inventar funções e parâmetros que parecem plausíveis.

## Validação

Respostas, códigos e recomendações devem ser analisados antes da utilização prática.

## Qualidade dos dados

A qualidade do modelo semântico influencia a capacidade de ferramentas de IA compreenderem o contexto dos dados.

## Segurança

Informações confidenciais e propriedade intelectual devem ser tratadas de acordo com as políticas de segurança da organização.

## Limites técnicos

Determinados recursos podem possuir requisitos de capacidade, disponibilidade, infraestrutura e limites de entrada.

## Principal aprendizado

> **Uma resposta bem escrita não significa necessariamente uma resposta correta.**

---

# 9. 🧪 O que os experimentos demonstraram

Durante o projeto foram realizados quatro experimentos principais.

## Experimento 01

**Objetivo:** mapear os conhecimentos das cinco fontes.

**Resultado:** foi possível relacionar IA Generativa, Engenharia de Prompts, Power BI, Copilot e DAX.

---

## Experimento 02

**Objetivo:** validar as informações produzidas pelo primeiro experimento.

**Resultado:** algumas afirmações precisaram de ajustes de contexto e precisão.

---

## Experimento 03

**Objetivo:** estudar aplicações de IA Generativa relacionadas ao DAX.

**Resultado:** a IA apresentou diversas possibilidades de apoio, mas também produziu informações adicionais que precisaram ser verificadas.

---

## Experimento 04

**Objetivo:** comparar prompt simples e prompt estruturado.

**Resultado:** o prompt estruturado produziu uma resposta mais contextualizada e útil.

## Conclusão dos experimentos

Os testes demonstraram que:

**Contexto + Objetivo + Restrições + Formato**

ajudam a melhorar o controle sobre a resposta produzida pela IA.

Ao mesmo tempo:

**Prompt melhor ≠ resposta automaticamente correta**

A validação continua sendo necessária.

---

# 10. 🩹 Principais cicatrizes de aprendizagem

## 1. Restrição de fonte

Uma fonte oficial inicialmente selecionada não foi aceita pelo NotebookLM devido a restrições de acesso.

**Aprendizado:** fontes disponíveis na Internet podem apresentar limitações de importação em determinadas ferramentas.

## 2. Contexto

Uma informação verdadeira foi inicialmente apresentada em um contexto inadequado.

**Aprendizado:** é necessário avaliar a informação e também o contexto em que ela está sendo utilizada.

## 3. Extrapolação

Mesmo com instruções para utilizar exclusivamente as fontes, a IA apresentou informações adicionais.

**Aprendizado:** a resposta precisa ser comparada com as fontes.

## 4. Prompt estruturado

O prompt estruturado apresentou um resultado mais direcionado ao objetivo.

**Aprendizado:** fornecer contexto, objetivo, restrições e formato melhora o controle da interação.

---

# 11. 📚 Glossário

| Conceito                  | Definição                                                                           |
| ------------------------- | ----------------------------------------------------------------------------------- |
| **IA Generativa**         | Tecnologia capaz de gerar novos conteúdos a partir de instruções                    |
| **LLM**                   | Large Language Model, modelo de linguagem de grande escala                          |
| **Deep Learning**         | Aprendizado baseado em redes neurais profundas                                      |
| **Transformer**           | Arquitetura utilizada em muitos modelos modernos de IA                              |
| **Atenção**               | Mecanismo utilizado para considerar relações entre partes de uma sequência          |
| **Modelo de Base**        | Modelo treinado em grandes volumes de dados e adaptável a tarefas                   |
| **Fine-tuning**           | Processo de adaptação de um modelo para determinada tarefa                          |
| **RAG**                   | Técnica que utiliza recuperação de informações externas para complementar a geração |
| **Prompt**                | Instrução fornecida a um modelo de IA                                               |
| **Engenharia de Prompts** | Processo de criação e aperfeiçoamento de prompts                                    |
| **Zero-shot**             | Solicitação sem exemplos prévios                                                    |
| **Few-shot**              | Solicitação com alguns exemplos                                                     |
| **Chain of Thought**      | Técnica apresentada para decompor problemas complexos em etapas                     |
| **Power BI**              | Plataforma de análise e visualização de dados                                       |
| **Modelo Semântico**      | Estrutura que organiza dados e relacionamentos para análise                         |
| **Copilot**               | Assistente baseado em IA integrado a produtos Microsoft                             |
| **DAX**                   | Linguagem de expressões para modelos de dados tabulares                             |
| **Medida**                | Cálculo DAX avaliado dinamicamente                                                  |
| **Coluna Calculada**      | Coluna criada por uma expressão DAX                                                 |
| **Tabela Calculada**      | Tabela criada por uma expressão DAX                                                 |
| **RLS**                   | Segurança em nível de linha                                                         |
| **Contexto de Filtro**    | Conjunto de filtros que afetam um cálculo                                           |
| **Contexto de Linha**     | Linha atualmente avaliada por uma expressão                                         |

---

# 12. 🧰 Prompts reutilizáveis

## Estudar um conceito

```text
Explique o conceito de [CONCEITO] utilizando exclusivamente
as fontes disponíveis.

Apresente:
1. Definição;
2. Principais características;
3. Exemplo prático;
4. Aplicação profissional;
5. Limitações;
6. Fonte utilizada.

Não utilize informações externas às fontes.
```

---

## Validar uma resposta

```text
Analise criticamente a resposta abaixo utilizando
exclusivamente as fontes disponíveis.

Classifique cada afirmação como:

- Confirmada;
- Parcialmente confirmada;
- Não confirmada.

Para cada afirmação, indique a fonte correspondente
e explique o motivo da classificação.

Não complete informações que não estejam presentes nas fontes.
```

---

## Estudar Power BI

```text
Atue como professor de Power BI.

Explique [TEMA] considerando:

1. Conceito;
2. Finalidade;
3. Exemplo;
4. Aplicação profissional;
5. Erros comuns;
6. Pontos que precisam ser validados.

Priorize informações sustentadas pelas fontes disponíveis.
```

---

## Estudar DAX

```text
Atue como especialista em Power BI e DAX.

Explique [FUNÇÃO OU CONCEITO].

Apresente:
1. O que é;
2. Para que serve;
3. Sintaxe;
4. Exemplo;
5. Influência do contexto;
6. Erros comuns;
7. Como validar o resultado.

Não invente funções ou parâmetros.
```

---

## Comparar prompts

```text
Compare os dois prompts abaixo.

Prompt A:
[INSIRA PROMPT]

Prompt B:
[INSIRA PROMPT]

Avalie:
- clareza;
- contexto;
- especificidade;
- restrições;
- formato de saída;
- controle da resposta;
- utilidade prática.

Explique qual apresenta maior capacidade de direcionamento e por quê.
```

---

# 🎓 13. Principais aprendizados

Ao final do projeto, os principais aprendizados foram:

1. A Inteligência Artificial pode ser utilizada como ferramenta de aprendizagem ativa.
2. A curadoria de fontes é fundamental para construir uma base confiável de estudo.
3. Contexto e clareza melhoram a qualidade das interações com a IA.
4. Prompts estruturados podem produzir respostas mais direcionadas.
5. Respostas geradas pela IA precisam ser verificadas.
6. A qualidade dos dados influencia aplicações de IA na análise de dados.
7. O Power BI e o DAX possuem fundamentos técnicos que precisam ser compreendidos pelo profissional.
8. O Copilot pode apoiar diversas atividades relacionadas a dados e DAX.
9. A IA pode acelerar atividades, mas não substitui a responsabilidade técnica do analista.
10. O principal diferencial está na combinação entre conhecimento técnico, uso consciente da IA e pensamento crítico.

---

# 💡 Conclusão

O desenvolvimento deste Caderno Temático demonstrou que a Inteligência Artificial pode ser utilizada como ferramenta de pesquisa, aprendizagem, experimentação e organização do conhecimento.

A combinação entre Inteligência Artificial Generativa, Engenharia de Prompts, Power BI, Copilot e DAX apresenta possibilidades importantes para o profissional de análise de dados.

Entretanto, o projeto também mostrou que utilizar IA de forma eficiente exige mais do que saber fazer perguntas.

É necessário:

**perguntar → analisar → verificar → questionar → refinar → validar → aprender**

A principal conclusão é:

> **A melhor utilização da Inteligência Artificial não consiste em aceitar respostas prontas, mas em saber fazer perguntas melhores, avaliar criticamente as respostas e transformar a interação com a IA em conhecimento.**

---

## 👨‍💻 Autor

**Frederico de Azevedo Werneck**

Projeto desenvolvido como atividade prática de aprendizagem e construção de portfólio na DIO.

---

**Status: Projeto concluído ✅**
