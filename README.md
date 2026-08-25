# 🤖 Inteligência Artificial Generativa aplicada à Análise de Dados com Power BI e DAX

## 📌 Sobre o projeto

Este projeto foi desenvolvido como parte de um desafio da DIO, com o objetivo de explorar a Inteligência Artificial como ferramenta de aprendizagem ativa.

O tema escolhido foi a aplicação da **Inteligência Artificial Generativa na Análise de Dados**, com foco em **Microsoft Power BI, Copilot e linguagem DAX**.

Durante o desenvolvimento, utilizei o **NotebookLM** para organizar fontes oficiais, comparar informações, elaborar perguntas, testar diferentes abordagens de prompts e consolidar os conhecimentos adquiridos em um miniguia de estudos.

O projeto também busca demonstrar como a IA pode ser utilizada de maneira crítica e responsável, não apenas para gerar respostas, mas como ferramenta de apoio à pesquisa, aprendizagem, análise e validação de informações.

---

## 🎯 Objetivos

Os principais objetivos deste projeto são:

- Compreender os fundamentos da Inteligência Artificial Generativa;
- Entender os principais conceitos relacionados à Engenharia de Prompts;
- Estudar a utilização da Inteligência Artificial aplicada à análise de dados;
- Aprofundar os conhecimentos sobre Microsoft Power BI;
- Compreender o funcionamento e as aplicações do Copilot no Power BI;
- Revisar conceitos fundamentais da linguagem DAX;
- Explorar como a IA pode auxiliar na criação e documentação de expressões DAX;
- Identificar limitações, riscos e cuidados no uso de IA generativa;
- Desenvolver prompts reutilizáveis para apoiar estudos e atividades futuras;
- Consolidar o conhecimento em um miniguia de estudos.

---

# 📚 1. Curadoria das fontes

Para desenvolver o projeto, foram selecionadas cinco fontes oficiais e abertas relacionadas aos temas estudados.

As fontes foram inseridas no NotebookLM para análise, comparação e geração de conhecimento.

### Fonte 1 — IBM

**Tema:** Inteligência Artificial Generativa

Material utilizado para estudar conceitos como:

- Inteligência Artificial Generativa;
- Deep Learning;
- Redes neurais;
- Modelos de base;
- Transformadores;
- Mecanismo de atenção;
- Fine-tuning;
- RAG (Retrieval-Augmented Generation);
- Limitações e riscos da IA generativa.

---

### Fonte 2 — Google Cloud

**Tema:** Engenharia de Prompts

Material utilizado para estudar:

- Engenharia de prompts;
- Zero-shot;
- One-shot;
- Few-shot;
- Multi-shot;
- Chain of Thought;
- Estruturação de instruções;
- Contextualização;
- Clareza e especificidade dos prompts;
- Estratégias para melhorar as respostas de modelos de IA.

---

### Fonte 3 — Microsoft Learn

**Tema:** Microsoft Power BI

Material utilizado para revisar:

- Power BI;
- Power BI Desktop;
- Modelos semânticos;
- Relatórios;
- Dashboards;
- Modelagem de dados;
- Relacionamentos;
- Esquema estrela;
- Preparação dos dados para utilização com IA.

---

### Fonte 4 — Microsoft Learn

**Tema:** Copilot no Power BI

Material utilizado para estudar:

- Copilot no Power BI;
- Utilização de IA em relatórios;
- Geração de consultas DAX;
- Geração de expressões DAX;
- Refinamento de medidas;
- Documentação de medidas;
- Experiências de Copilot;
- Preparação dos modelos semânticos;
- Limitações e requisitos de utilização.

---

### Fonte 5 — Microsoft Learn

**Tema:** Linguagem DAX

Material utilizado para revisar:

- Data Analysis Expressions (DAX);
- Medidas;
- Colunas calculadas;
- Tabelas calculadas;
- Segurança em nível de linha (RLS);
- Contexto de linha;
- Contexto de filtro;
- Variáveis;
- Funções e expressões DAX.

---

# 🧠 2. Mapa de conhecimentos

A análise das fontes permitiu identificar uma relação direta entre cinco grandes áreas:

| Tema | Papel no projeto |
|---|---|
| **IA Generativa** | Base tecnológica para geração de conteúdo e código |
| **Engenharia de Prompts** | Forma de comunicação e direcionamento da IA |
| **Power BI** | Ambiente utilizado para análise, modelagem e visualização dos dados |
| **Copilot no Power BI** | Aplicação prática da IA generativa dentro do Power BI |
| **DAX** | Linguagem utilizada para cálculos e consultas em modelos tabulares |

A conexão entre esses conhecimentos pode ser representada da seguinte forma:

**IA Generativa → Engenharia de Prompts → Copilot → Power BI → DAX → Análise de Dados**

Essa relação demonstra que a utilização eficiente da IA depende não apenas da ferramenta, mas também da qualidade dos dados, da modelagem e da capacidade do profissional de formular boas solicitações e validar os resultados.

---

# 🔎 3. Utilização do NotebookLM

O NotebookLM foi utilizado como ambiente de estudo e organização das fontes selecionadas.

As principais atividades realizadas foram:

1. Inserção das fontes oficiais;
2. Organização do material de referência;
3. Identificação dos principais conceitos;
4. Comparação entre as informações das diferentes fontes;
5. Elaboração de perguntas estratégicas;
6. Testes de diferentes prompts;
7. Análise crítica das respostas;
8. Identificação de informações que precisavam de ajustes;
9. Consolidação dos conhecimentos;
10. Construção do miniguia final.

Um dos pontos mais importantes do processo foi perceber que a resposta gerada pela IA precisa ser **analisada e validada**, mesmo quando apresenta uma resposta aparentemente correta.

---

# 🧪 4. Engenharia de Prompts

Durante o projeto foram realizados testes com diferentes níveis de detalhamento dos prompts.

## Prompt inicial

> Crie uma medida DAX para calcular o total de vendas.

A resposta apresentou uma solução simples, porém utilizou nomes de campos que não haviam sido especificados no contexto.

Isso mostrou a importância de fornecer informações suficientes para limitar a possibilidade de respostas inadequadas.

---

## Prompt refinado

> Atue como um especialista em Power BI e DAX.
>
> Com base exclusivamente nas fontes disponíveis neste notebook, proponha uma medida DAX para calcular o total de vendas.
>
> Contexto:
>
> - Existe uma tabela chamada Sales.
> - A tabela possui uma coluna chamada SalesAmount.
> - SalesAmount contém valores numéricos referentes às vendas.
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

O resultado obtido foi:

```DAX
Total Vendas = SUM('Sales'[SalesAmount])

Esse exemplo demonstrou como o fornecimento de contexto e a definição clara do objetivo podem melhorar significativamente a qualidade da resposta.

🩹 5. Cicatrizes e aprendizados durante o processo

Durante a construção do projeto foram identificados alguns pontos que exigiram revisão e validação.

5.1 Limite de caracteres

O limite de 10.000 caracteres por prompt foi identificado como uma característica específica do Copilot no Power BI.

Por isso, esse limite não deve ser apresentado como uma regra geral da Engenharia de Prompts.

5.2 Geração e otimização de DAX

Inicialmente foi utilizada a expressão "otimização e explicação de DAX".

Após a análise das fontes, a descrição foi ajustada para refletir com maior precisão as capacidades documentadas do Copilot, incluindo:

geração de expressões DAX;
escrita de consultas DAX;
refinamento de medidas;
criação de descrições para medidas.
5.3 Validação das respostas

Outro aprendizado importante foi perceber que uma resposta aparentemente correta pode conter informações que não estão necessariamente sustentadas pelas fontes utilizadas.

Por isso, uma etapa fundamental do projeto foi comparar as respostas geradas pela IA com a documentação oficial.

📖 6. Miniguia de Estudos
6.1 Inteligência Artificial Generativa

A Inteligência Artificial Generativa é uma área da Inteligência Artificial capaz de produzir novos conteúdos a partir de instruções fornecidas pelo usuário.

Entre os conteúdos que podem ser gerados estão:

textos;
imagens;
áudio;
vídeo;
código.

A tecnologia utiliza modelos de aprendizado profundo e redes neurais treinadas com grandes volumes de dados.

Conceitos importantes

Deep Learning: utilização de redes neurais para aprender padrões em grandes volumes de dados.

Modelos de base: modelos treinados com grandes conjuntos de dados que podem posteriormente ser adaptados para diferentes tarefas.

Transformadores: arquitetura utilizada por muitos modelos modernos de IA, baseada no mecanismo de atenção para compreender relações e contexto dentro das sequências.

Fine-tuning: processo de adaptação de um modelo para tarefas ou contextos específicos.

RAG: técnica que permite ao modelo consultar informações externas ao seu conjunto original de treinamento.

6.2 Engenharia de Prompts

Engenharia de Prompts consiste na criação e no aprimoramento das instruções fornecidas a modelos de Inteligência Artificial.

Um bom prompt deve apresentar:

objetivo claro;
contexto;
informações relevantes;
restrições;
formato esperado da resposta.
Principais técnicas

Zero-shot: solicitação realizada sem fornecer exemplos.

One-shot: utilização de um exemplo.

Few-shot: utilização de alguns exemplos para orientar o padrão esperado.

Chain of Thought: abordagem que orienta a resolução de problemas complexos em etapas.

Estrutura recomendada

Um prompt pode ser organizado da seguinte maneira:

Papel + Contexto + Objetivo + Restrições + Formato da resposta

6.3 Microsoft Power BI

O Power BI é uma plataforma utilizada para análise, modelagem e visualização de dados.

Entre seus principais elementos estão:

Power BI Desktop;
modelos semânticos;
relatórios;
dashboards;
relacionamentos;
visualizações;
gateways.

Uma boa modelagem dos dados é fundamental para a qualidade das análises.

O esquema estrela é uma abordagem importante para estruturar modelos analíticos.

6.4 Copilot no Power BI

O Copilot utiliza Inteligência Artificial Generativa para auxiliar usuários na realização de tarefas relacionadas ao Power BI.

Entre as possibilidades documentadas estão:

geração de consultas DAX;
geração de expressões DAX;
refinamento de medidas;
criação de descrições para medidas;
geração de resumos;
apoio na criação de relatórios;
interação com dados.

Um ponto fundamental identificado no estudo é que a qualidade do modelo semântico influencia diretamente a capacidade do Copilot de compreender o contexto dos dados.

6.5 DAX

DAX — Data Analysis Expressions é uma linguagem utilizada para realizar cálculos e consultas em modelos de dados tabulares.

No Power BI, DAX pode ser utilizado para criar:

Medidas

São cálculos avaliados dinamicamente de acordo com o contexto do relatório.

Exemplo:

Total Vendas = SUM('Sales'[SalesAmount])
Colunas calculadas

São calculadas linha a linha e armazenadas no modelo.

Tabelas calculadas

São tabelas criadas por meio de expressões DAX.

RLS

A Segurança em Nível de Linha permite definir quais registros podem ser visualizados de acordo com funções e permissões.

🧩 7. Conceito fundamental: contexto no DAX

O contexto é um dos conceitos mais importantes para compreender o funcionamento do DAX.

Contexto de linha

Representa a linha que está sendo avaliada.

Contexto de filtro

Representa as restrições aplicadas aos dados por meio de filtros, segmentações ou expressões.

Contexto de consulta

Está relacionado ao conjunto de dados solicitado por um visual ou consulta.

Compreender esses conceitos é fundamental para interpretar corretamente os resultados das medidas.

🤖 8. IA Generativa aplicada ao DAX

A Inteligência Artificial pode apoiar o profissional de dados em diversas atividades relacionadas ao DAX.

Possíveis aplicações
criação de rascunhos de medidas;
geração de consultas DAX;
refinamento de medidas;
documentação de medidas;
explicação de fórmulas;
apoio na identificação de erros;
organização da lógica de cálculos.

Entretanto, a IA deve ser utilizada como assistente, e não como substituta da validação técnica realizada pelo analista.

⚠️ 9. Limitações e cuidados

Durante o estudo foram identificados alguns cuidados importantes.

Alucinações

Modelos de IA podem gerar informações incorretas ou inventar funções e argumentos que parecem plausíveis.

Qualidade dos dados

Um modelo semântico mal estruturado pode prejudicar a qualidade das respostas geradas pela IA.

Segurança

Informações confidenciais e propriedade intelectual devem ser protegidas durante a utilização de ferramentas de IA.

Validação

Todo código gerado pela IA deve ser analisado, testado e validado antes de ser utilizado em um ambiente de produção.

Licenciamento

O uso do Copilot no Power BI possui requisitos específicos de capacidade e licenciamento documentados pela Microsoft.

Limite de prompt

O Copilot no Power BI possui limite documentado de 10.000 caracteres por prompt.

📚 10. Glossário
Conceito	Definição
IA Generativa	Tecnologia capaz de gerar novos conteúdos a partir de instruções
LLM	Modelo de linguagem de grande escala
Deep Learning	Aprendizado baseado em redes neurais profundas
Transformador	Arquitetura baseada em mecanismos de atenção
RAG	Técnica que utiliza fontes externas para complementar informações
Prompt	Instrução fornecida a um modelo de IA
Zero-shot	Prompt sem exemplos
Few-shot	Prompt com alguns exemplos
Chain of Thought	Técnica de decomposição de problemas em etapas
Power BI	Plataforma de análise e visualização de dados
Copilot	Assistente de IA integrado ao ecossistema Microsoft
DAX	Linguagem de expressões para modelos tabulares
Medida	Cálculo dinâmico realizado no modelo
Coluna calculada	Cálculo realizado para cada linha
Tabela calculada	Tabela criada por expressão DAX
RLS	Segurança em nível de linha
Modelo semântico	Estrutura que organiza dados, relacionamentos e lógica analítica
Esquema estrela	Modelo de dados baseado em tabelas fato e dimensões
Contexto de filtro	Conjunto de filtros que afetam um cálculo
Contexto de linha	Linha atualmente avaliada pelo DAX
♻️ 11. Prompts reutilizáveis
Criar uma medida DAX
Atue como especialista em Power BI e DAX.

Com base nas informações fornecidas, crie uma medida DAX.

Tabela:
[Nome da tabela]

Colunas disponíveis:
[Nome das colunas]

Objetivo:
[Descreva o cálculo]

Apresente:
1. Código DAX;
2. Explicação da lógica;
3. Tipo de objeto criado;
4. Pontos que precisam ser validados pelo analista.

Não invente nomes de tabelas ou colunas.
Explicar uma medida DAX
Explique a seguinte medida DAX de forma didática:

[CÓDIGO DAX]

Apresente:
1. Objetivo da medida;
2. Funções utilizadas;
3. Lógica do cálculo;
4. Influência do contexto de filtro;
5. Possíveis pontos de atenção.
Revisar uma medida DAX
Analise a seguinte medida DAX:

[CÓDIGO]

Verifique:
1. Sintaxe;
2. Funções utilizadas;
3. Referências às tabelas e colunas;
4. Possíveis problemas de contexto;
5. Resultado esperado;
6. Sugestões de melhoria.

Não altere a lógica de negócio sem explicar a alteração.
Estudar um conceito
Explique o conceito de [CONCEITO] no contexto do Power BI e DAX.

Apresente:
1. Definição;
2. Exemplo simples;
3. Aplicação prática;
4. Erros comuns;
5. Uma pergunta para testar meu conhecimento.
🎓 12. Principais aprendizados

O desenvolvimento deste projeto permitiu consolidar alguns aprendizados importantes:

A Inteligência Artificial Generativa pode ser uma importante ferramenta de aprendizagem e produtividade.
A qualidade do prompt influencia diretamente a qualidade da resposta.
O contexto fornecido à IA é fundamental para reduzir ambiguidades.
A qualidade e organização dos dados são essenciais para aplicações de IA em análise de dados.
O Power BI utiliza DAX como linguagem fundamental para cálculos e consultas em modelos tabulares.
O Copilot pode auxiliar em diversas tarefas relacionadas ao Power BI e DAX.
Respostas geradas por IA precisam ser analisadas e validadas.
A IA não substitui o conhecimento técnico e a responsabilidade do profissional.
A documentação oficial deve ser utilizada como referência para validação de informações.
O uso consciente da IA combina automação, pensamento crítico e conhecimento técnico.
🚀 13. Conclusão

O desenvolvimento deste projeto demonstrou que a Inteligência Artificial pode ser utilizada de forma prática como ferramenta de aprendizagem ativa.

A combinação entre IA Generativa, Engenharia de Prompts, Power BI, Copilot e DAX apresenta oportunidades importantes para aumentar a produtividade do profissional de análise de dados.

Ao mesmo tempo, o projeto reforçou que a utilização da IA exige pensamento crítico, validação das informações, qualidade dos dados e conhecimento técnico.

O principal aprendizado foi compreender que o profissional não deve simplesmente aceitar a resposta produzida pela IA. Ele deve saber formular a pergunta, analisar a resposta, confrontá-la com fontes confiáveis e validar tecnicamente o resultado.

Dessa forma, a IA passa a atuar como uma ferramenta de apoio ao desenvolvimento profissional, enquanto a tomada de decisão e a responsabilidade técnica continuam sob o controle do analista.

🤖 14. Uso de Inteligência Artificial

A Inteligência Artificial foi utilizada como ferramenta de apoio durante o desenvolvimento deste projeto, principalmente para:

organização das informações;
elaboração e refinamento de prompts;
análise das respostas;
identificação de pontos que precisavam de revisão;
estruturação do material de estudo;
consolidação dos conhecimentos.

As informações técnicas foram confrontadas com as fontes oficiais selecionadas e utilizadas no NotebookLM.

O objetivo foi utilizar a IA como ferramenta de aprendizagem, pesquisa e organização do conhecimento, mantendo a análise crítica e a validação das informações como responsabilidade do autor do projeto.

👨‍💻 Autor

Frederico de Azevedo Werneck

Projeto desenvolvido para o desafio da DIO — Inteligência Artificial como ferramenta de aprendizagem ativa.

⭐ Projeto desenvolvido com foco em Inteligência Artificial, Análise de Dados, Power BI, DAX e Engenharia de Prompts.
