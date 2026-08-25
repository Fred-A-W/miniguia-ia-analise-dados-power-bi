# 🧠 Engenharia de Prompts e Experimentos

Este arquivo registra os principais experimentos realizados durante o desenvolvimento do Caderno Temático no NotebookLM.

O objetivo foi compreender, na prática, como diferentes estratégias de elaboração de prompts influenciam as respostas produzidas pela Inteligência Artificial e como a validação crítica pode melhorar a qualidade do processo de aprendizagem.

---

# 🔬 Experimento 01 — Mapeamento inicial dos conhecimentos

## Objetivo

Identificar os principais conceitos presentes nas cinco fontes utilizadas no NotebookLM e compreender como os temas de Inteligência Artificial Generativa, Engenharia de Prompts, Power BI, Copilot e DAX estão relacionados.

## Prompt utilizado

> Analise todas as cinco fontes disponíveis neste notebook e construa um mapa inicial dos conhecimentos abordados.
>
> Organize a resposta em uma tabela com as seguintes colunas:
>
> 1. Tema principal
> 2. Conceitos fundamentais
> 3. Fonte(s) que abordam o tema
> 4. Relação do tema com os demais conteúdos
> 5. Aplicação prática para um profissional de análise de dados
>
> Não utilize informações externas às fontes disponíveis no notebook.
>
> Ao final, apresente uma síntese explicando como os cinco conteúdos se conectam dentro do tema central "Inteligência Artificial Generativa aplicada à Análise de Dados e Power BI".
>
> Sempre que possível, indique a fonte utilizada para sustentar cada informação.

## Resultado

O NotebookLM identificou cinco grandes áreas de conhecimento:

* Inteligência Artificial Generativa;
* Engenharia de Prompts;
* Microsoft Power BI;
* Copilot no Power BI;
* DAX.

A resposta também estabeleceu uma relação entre os temas, mostrando que a IA Generativa representa a base tecnológica, a Engenharia de Prompts representa a forma de interação, o Power BI funciona como ambiente de análise, o Copilot conecta IA ao Power BI e o DAX fornece a linguagem utilizada para cálculos e consultas em modelos tabulares.

## Aprendizado

O NotebookLM mostrou-se útil para organizar informações presentes em diferentes fontes e estabelecer conexões entre conceitos.

---

# 🔎 Experimento 02 — Validação crítica

## Objetivo

Verificar se as informações apresentadas no primeiro experimento estavam realmente sustentadas pelas cinco fontes utilizadas.

## Prompt utilizado

> Analise criticamente a resposta apresentada anteriormente no Prompt 01.
>
> Utilize exclusivamente as cinco fontes disponíveis neste notebook para realizar a validação.
>
> Para cada uma das principais afirmações apresentadas na resposta anterior, classifique-a em uma das seguintes categorias:
>
> * CONFIRMADA: a informação está claramente sustentada por uma das fontes.
> * PARCIALMENTE CONFIRMADA: a fonte aborda o assunto, mas a resposta anterior acrescentou detalhes ou interpretações que não estão claramente sustentados.
> * NÃO CONFIRMADA: não foi possível localizar sustentação suficiente nas fontes disponíveis.
>
> Organize o resultado em uma tabela contendo:
>
> 1. Afirmação analisada
> 2. Classificação
> 3. Fonte que sustenta a afirmação
> 4. Evidência ou explicação encontrada na fonte
> 5. Observação sobre possíveis exageros, interpretações ou informações que precisam ser verificadas
>
> Não complete lacunas com conhecimento externo. Quando uma informação não puder ser confirmada pelas fontes, declare explicitamente que ela não foi localizada ou não está suficientemente sustentada.

## Principais descobertas

O processo de validação confirmou a maior parte das informações, mas também mostrou a importância de utilizar cada informação dentro do contexto correto.

Um exemplo foi o limite de **10.000 caracteres por prompt**, identificado como uma característica específica do Copilot no Power BI e não como uma regra geral da Engenharia de Prompts.

Também foi identificado que determinadas afirmações relacionadas ao DAX precisavam de maior precisão terminológica.

## Aprendizado

Uma informação pode estar correta e ainda assim ser apresentada no contexto inadequado.

A validação das respostas deve considerar:

**informação + fonte + contexto + aplicação.**

---

# 💼 Experimento 03 — IA Generativa aplicada ao DAX

## Objetivo

Investigar como a Inteligência Artificial Generativa pode apoiar um profissional de análise de dados em atividades relacionadas à linguagem DAX.

## Prompt utilizado

> Atue como um especialista em análise de dados e Power BI.
>
> Com base exclusivamente nas fontes disponíveis neste notebook, explique como a Inteligência Artificial Generativa pode apoiar um profissional na criação, compreensão e refinamento de expressões DAX.
>
> Organize a resposta nas seguintes seções:
>
> 1. O que é DAX e qual é sua função no Power BI;
> 2. Como a IA Generativa pode apoiar o trabalho com DAX;
> 3. Quais tipos de atividades relacionadas a DAX podem receber apoio da IA;
> 4. Quais cuidados o analista deve ter ao utilizar IA para gerar ou modificar expressões DAX;
> 5. Quais limitações devem ser consideradas;
> 6. Um exemplo hipotético de solicitação que um analista poderia fazer à IA para obter auxílio com DAX.
>
> Para cada afirmação importante, indique qual fonte do notebook a sustenta.
>
> Não invente funções, fórmulas ou recursos que não estejam sustentados pelas fontes.
>
> Diferencie claramente:
>
> * o que as fontes afirmam diretamente;
> * o que pode ser considerado uma aplicação prática;
> * o que representa uma interpretação ou recomendação.

## Resultado

A resposta apresentou aplicações relacionadas a:

* geração de expressões DAX;
* criação de consultas DAX;
* refinamento de medidas;
* documentação de medidas;
* apoio à compreensão de fórmulas.

Também apresentou cuidados relacionados à qualidade dos dados, preparação do modelo semântico, alucinações e necessidade de validação.

## Ponto de atenção

Mesmo com a instrução para utilizar exclusivamente as fontes, a resposta trouxe informações adicionais que precisaram ser analisadas.

Isso demonstrou que uma resposta detalhada pode conter informações além do escopo solicitado.

## Aprendizado

O uso de uma restrição no prompt ajuda a direcionar a resposta, mas **não elimina a necessidade de validação humana**.

---

# 🧪 Experimento 04 — Prompt simples × Prompt estruturado

## Objetivo

Comparar os resultados obtidos utilizando um prompt simples e um prompt estruturado para a mesma tarefa.

---

## Prompt A — Simples

> Crie uma medida DAX para calcular o total de vendas.

### Resultado

A resposta apresentou:

```DAX
Total Sales = SUM([Sales Amount])
```

O problema observado foi a ausência de contexto sobre a tabela e a coluna que deveriam ser utilizadas.

---

## Prompt B — Estruturado

> Atue como um especialista em Power BI e DAX.
>
> Com base exclusivamente nas fontes disponíveis neste notebook, proponha uma medida DAX para calcular o total de vendas.
>
> Contexto:
>
> * Existe uma tabela chamada Sales.
> * A tabela possui uma coluna chamada SalesAmount.
> * SalesAmount contém valores numéricos referentes às vendas.
>
> Objetivo:
>
> Criar uma medida chamada Total Vendas que calcule a soma dos valores de SalesAmount.
>
> Apresente:
>
> 1. O código DAX;
> 2. Uma explicação objetiva do funcionamento da medida;
> 3. O tipo de objeto criado;
> 4. Quais informações do contexto fornecido são necessárias para construir a medida;
> 5. Quais aspectos devem ser validados pelo analista antes de utilizar a medida em um relatório.
>
> Não invente nomes de tabelas, colunas ou funções além das informações fornecidas e não utilize informações externas às fontes disponíveis no notebook.

### Resultado

A resposta apresentou:

```DAX
Total Vendas = SUM('Sales'[SalesAmount])
```

Além do código, a resposta explicou o funcionamento da medida, identificou o objeto como uma medida e apresentou pontos de validação.

---

# 📊 Comparação dos experimentos

| Critério                 | Prompt simples | Prompt estruturado  |
| ------------------------ | -------------- | ------------------- |
| Clareza                  | Média          | Alta                |
| Contexto                 | Baixo          | Alto                |
| Especificidade           | Baixa          | Alta                |
| Controle da resposta     | Baixo          | Alto                |
| Formato de saída         | Não definido   | Definido            |
| Utilidade profissional   | Média          | Alta                |
| Necessidade de validação | Alta           | Continua necessária |

## Conclusão

O prompt estruturado produziu uma resposta mais contextualizada e adequada ao objetivo porque apresentou:

* papel do modelo;
* contexto;
* informações sobre os dados;
* objetivo;
* formato esperado;
* critérios de validação;
* restrições.

O experimento demonstrou, na prática, que **contexto, clareza, especificidade e restrições ajudam a melhorar o controle sobre a resposta gerada pela IA**.

Ao mesmo tempo, o experimento reforçou que um prompt mais elaborado **não elimina a necessidade de análise e validação humana**.

---

# 🩹 Cicatrizes de aprendizagem

## Cicatriz 01 — Restrição de fonte

Uma fonte oficial inicialmente selecionada não foi aceita pelo NotebookLM devido a restrições de acesso.

**Aprendizado:** uma fonte oficial disponível na Internet pode não ser compatível com a importação direta para determinada ferramenta.

---

## Cicatriz 02 — Contexto da informação

Uma informação verdadeira foi inicialmente apresentada de forma muito ampla.

**Aprendizado:** é necessário avaliar não apenas se a informação é verdadeira, mas também se está sendo apresentada no contexto correto.

---

## Cicatriz 03 — Extrapolação da IA

Mesmo com a orientação de utilizar exclusivamente as fontes disponíveis, algumas respostas apresentaram informações adicionais que exigiram validação.

**Aprendizado:** respostas detalhadas e convincentes ainda precisam ser verificadas.

---

## Cicatriz 04 — Prompt simples versus estruturado

O prompt estruturado apresentou um resultado mais contextualizado.

**Aprendizado:** o usuário precisa saber fornecer contexto, objetivo, restrições e formato de saída para obter respostas mais adequadas.

---

# 🧠 Principais aprendizados sobre Engenharia de Prompts

Ao final dos experimentos, os principais aprendizados foram:

1. Um prompt claro reduz ambiguidades.
2. Contexto é fundamental para direcionar a resposta.
3. Definir o formato de saída aumenta o controle sobre o resultado.
4. Restrições podem ajudar a manter a resposta dentro do objetivo.
5. Prompts mais detalhados podem produzir respostas mais úteis.
6. Respostas geradas pela IA precisam ser validadas.
7. A utilização de fontes confiáveis aumenta a qualidade do processo de aprendizagem.
8. O usuário continua responsável pela análise crítica e validação do resultado.

---

# 🎯 Modelo reutilizável de prompt

A partir dos experimentos realizados, foi identificado o seguinte modelo como referência:

```text
Atue como [PAPEL].

Contexto:
[INFORMAÇÕES RELEVANTES]

Objetivo:
[O QUE PRECISO OBTER]

Tarefa:
[O QUE DEVE SER FEITO]

Restrições:
[O QUE NÃO DEVE SER FEITO]

Formato da resposta:
[COMO A RESPOSTA DEVE SER APRESENTADA]

Critérios de validação:
[COMO DEVO AVALIAR O RESULTADO]
```

Esse modelo pode ser adaptado para estudos, análise de dados, Power BI, DAX e outras atividades profissionais.

---

# ✅ Conclusão

Os experimentos demonstraram que a Engenharia de Prompts não consiste apenas em escrever perguntas mais longas.

Ela envolve compreender:

* o objetivo;
* o contexto;
* as informações disponíveis;
* as limitações da ferramenta;
* o formato desejado;
* os critérios de validação.

O principal aprendizado foi que uma boa interação com a Inteligência Artificial exige participação ativa do usuário.

> **Perguntar melhor é importante, mas validar melhor é indispensável.**
