# Material integral do guia técnico

> Esta página preserva o texto consolidado do guia técnico integrado em formato navegável. As demais páginas do site reorganizam esse conteúdo como wiki didática, com trilhas, conceitos, métricas, templates e aplicações.

[Baixar o DOCX-fonte](../assets/fontes/Guia_Tecnico_Metodologico_Integrado_Final.docx)

---

## Guia Técnico-Metodológico para Formalização, Implementação e Validação de Frameworks, Arquiteturas, Métodos, Metodologias, Modelos, Pipelines, Plataformas, Agentes e Artefatos Computacionais

### Documento-base para Iniciação Científica, Mestrado e Doutorado em Ciência da Computação

## 1. Apresentação

Este guia técnico-metodológico tem como finalidade orientar a concepção, formalização, implementação, documentação, validação e avaliação de propostas acadêmicas em Ciência da Computação que envolvam frameworks, arquiteturas, métodos, metodologias, modelos, pipelines de dados, plataformas computacionais, agentes inteligentes e artefatos digitais.

O documento foi elaborado para apoiar estudantes de Iniciação Científica, Mestrado e Doutorado na transformação de uma ideia inicial em uma proposta científica tecnicamente consistente, metodologicamente defensável, avaliável, rastreável e reprodutível. Em muitos trabalhos acadêmicos, propostas computacionais são inicialmente apresentadas apenas por meio de figuras conceituais, fluxos genéricos ou descrições amplas. Embora essas representações sejam importantes, elas não são suficientes para caracterizar uma contribuição científica robusta.

Uma proposta computacional precisa explicitar o que está sendo criado, por que está sendo criado, qual lacuna pretende enfrentar, quais elementos a compõem, como esses elementos se relacionam, quais artefatos são produzidos, quais metadados devem ser registrados, quais critérios de qualidade serão utilizados, como será implementada, como será validada e como poderá ser replicada, avaliada ou evoluída por outros pesquisadores.

Este guia parte da premissa de que uma contribuição em Ciência da Computação pode assumir diferentes formas: um modelo, um modelo de referência, um método, uma técnica, uma metodologia, uma arquitetura, um framework, um framework técnico-metodológico, uma plataforma, um pipeline, um protótipo, um agente inteligente, um catálogo, um dashboard, um repositório, um guia, um template ou um conjunto integrado de artefatos. Cada tipo de contribuição possui natureza, escopo, forma de validação e critérios de avaliação distintos.

O guia utiliza exemplos inspirados em propostas em desenvolvimento, como EdmLens, MILA-eDU, UnespDataLens, SemED-LLM, FairED-Pipeline, GeoReXAI, EduPipeX e outras iniciativas relacionadas a dados educacionais, inteligência artificial, explicabilidade, governança, semântica, vieses, agentes inteligentes, mineração de dados educacionais, análise geoespacial e arquiteturas analíticas.

O objetivo não é transformar todos os projetos em uma mesma estrutura, mas oferecer um roteiro para que cada proposta seja formalizada de acordo com sua natureza. Um framework não deve ser descrito como se fosse apenas um método. Uma arquitetura não deve ser tratada como se fosse uma metodologia. Uma plataforma não deve ser confundida com um modelo de referência. Um agente inteligente não deve aparecer apenas como uma caixa de “IA” em um diagrama. Cada artefato precisa ter identidade conceitual, técnica e metodológica.

## 2. Finalidade do guia

A finalidade deste guia é oferecer um roteiro para formalizar propostas computacionais de forma clara, sistemática e avaliável.

O guia busca apoiar o pesquisador a responder às seguintes perguntas:

O que exatamente está sendo proposto?

A proposta é um framework, uma arquitetura, uma metodologia, um método, uma técnica, um modelo, uma plataforma, um pipeline, um sistema, um agente ou um artefato?

Qual lacuna científica, técnica, metodológica, arquitetural ou aplicada justifica a proposta?

Qual é a contribuição para Ciência da Computação?

Quais conceitos precisam ser definidos?

Quais módulos, componentes ou etapas compõem a proposta?

Quais artefatos são produzidos ou consumidos?

Quais metadados devem ser registrados?

Quais contratos existem entre módulos, dados, modelos, agentes ou artefatos?

Quais dimensões transversais precisam ser consideradas?

Como a proposta será implementada, instanciada ou demonstrada?

Como será validada?

Como será avaliada?

Como poderá ser documentada, replicada, reutilizada e evoluída?

O guia também busca evitar problemas recorrentes em trabalhos acadêmicos, como:

uso impreciso dos termos framework, arquitetura, método, metodologia, modelo, pipeline e plataforma;

propostas descritas apenas por diagramas;

módulos sem entradas e saídas definidas;

ausência de critérios de avaliação;

falta de rastreabilidade;

ausência de metadados;

ausência de contratos;

pouca preocupação com governança;

pouca preocupação com reprodutibilidade;

validação limitada apenas a um exemplo ilustrativo;

ausência de relação clara entre lacuna, objetivo, artefato e avaliação.

## 3. Público-alvo

Este guia pode ser utilizado por:

alunos de Iniciação Científica que precisam delimitar um artefato computacional inicial;

alunos de Mestrado que precisam propor, implementar e avaliar uma solução computacional;

alunos de Doutorado que precisam formalizar uma contribuição mais ampla, generalizável e avaliável;

orientadores que desejam padronizar a especificação de propostas;

grupos de pesquisa que desenvolvem frameworks, arquiteturas, plataformas, pipelines ou agentes;

equipes técnicas que precisam documentar artefatos computacionais reutilizáveis.

## 4. Níveis de profundidade conforme o tipo de pesquisa

A profundidade esperada depende do nível acadêmico da proposta.

| Nível | Característica da proposta | Produto esperado |

| --- | --- | --- |

| Iniciação Científica | Recorte delimitado, foco em aprendizado, protótipo parcial ou módulo específico | Especificação simplificada, implementação parcial, avaliação inicial |

| Mestrado | Proposta com implementação e avaliação em cenário delimitado | Framework, método, arquitetura, modelo ou protótipo validado em estudo de caso |

| Doutorado | Contribuição técnico-científica mais ampla, formalizada e avaliável | Framework técnico-metodológico, modelo de referência, arquitetura modular, especificação detalhada, avaliação multicritério e possibilidade de generalização |

No caso de uma Iniciação Científica, por exemplo, um aluno pode desenvolver um módulo de monitoramento de qualidade para pipelines educacionais. No Mestrado, pode propor e avaliar um framework de diagnóstico semântico com LLMs. No Doutorado, pode formalizar um framework técnico-metodológico completo, com modelo de referência, arquitetura modular, artefatos, metadados, contratos e avaliação multicritério.

## 5. Conceitos fundamentais

A precisão conceitual é o primeiro passo para uma boa proposta científica. Antes de desenhar uma arquitetura ou escrever módulos, o pesquisador precisa definir que tipo de artefato está propondo.

### 5.1 Modelo

Modelo é uma representação abstrata de um fenômeno, estrutura, processo, dado, comportamento ou sistema. Um modelo pode ser conceitual, matemático, computacional, semântico, estatístico, preditivo, causal, arquitetural ou de referência.

| Projeto | Exemplo de modelo | Papel na proposta |

| --- | --- | --- |

| EdmLens | Modelo de referência para pipelines de dados educacionais | Formalizar princípios, módulos, artefatos, metadados e critérios |

| MILA-eDU | Modelo analítico para apoio à decisão educacional | Representar fatores associados à evasão e possibilidades de intervenção |

| UnespDataLens | Modelo semântico de conceitos e módulos | Organizar conhecimento, links, termos e relações entre temas |

| SemED-LLM | Modelo de classificação semântica de interações estudantis | Representar lacunas conceituais em textos de estudantes |

| FairED-Pipeline | Modelo de categorias de vieses em pipelines educacionais | Organizar tipos de vieses por etapa do pipeline |

| GeoReXAI | Modelo geoespacial explicável | Relacionar dados espaciais, predições e explicações |

| EduPipeX | Modelo de explicabilidade de pipelines | Representar transformações, decisões técnicas e justificativas |

Um modelo não precisa necessariamente ser implementado como software completo. Ele pode servir para representar, organizar, explicar ou formalizar uma estrutura.

### 5.2 Modelo de referência

Modelo de referência é um tipo específico de modelo. Ele define uma estrutura geral, abstrata e reutilizável para orientar diferentes implementações ou instanciações de uma classe de soluções.

Um modelo de referência deve indicar:

princípios;

componentes essenciais;

artefatos;

metadados;

relações;

contratos;

critérios;

regras;

dimensões transversais;

possibilidades de adaptação.

Exemplos:

No EdmLens, um modelo de referência pode definir que todo pipeline educacional aderente deve possuir fontes inventariadas, extrações documentadas, transformações rastreáveis, integração controlada, armazenamento versionado, features documentadas, modelos avaliados, explicações registradas, governança, proveniência, monitoramento e catálogo.

No UnespDataLens, um modelo de referência pode definir como conceitos, métodos, técnicas, módulos, exemplos, glossários e relações devem ser organizados em uma plataforma navegável de conhecimento.

No FairED-Pipeline, um modelo de referência pode definir como identificar, medir, mitigar, registrar e monitorar vieses em diferentes etapas de um pipeline.

### 5.3 Método

Método é um procedimento sistemático para realizar uma tarefa específica. Ele possui um objetivo operacional claro e pode ser aplicado dentro de um módulo, metodologia ou framework.

| Projeto | Método | Função |

| --- | --- | --- |

| EdmLens | Validação de schema | Verificar conformidade estrutural dos dados |

| MILA-eDU | Associação estatística | Identificar relações entre variáveis educacionais e evasão |

| SemED-LLM | Prompting estruturado | Conduzir a classificação semântica de interações |

| FairED-Pipeline | Cálculo de Statistical Parity Difference | Medir diferença de resultados entre grupos |

| GeoReXAI | SHAP espacial | Explicar predições associadas a variáveis geoespaciais |

| EduPipeX | Reconstrução de pipeline | Explicar transformações aplicadas aos dados |

Um método pode ser validado por sua eficácia, precisão, consistência, custo computacional, aplicabilidade ou comparação com outros métodos.

### 5.4 Técnica

Técnica é uma forma específica de aplicar um método. Técnicas são mais operacionais e geralmente estão associadas a algoritmos, procedimentos computacionais ou estratégias práticas.

Exemplos de técnicas:

imputação de valores ausentes;

normalização;

padronização;

one-hot encoding;

anonimização;

pseudonimização;

SMOTE;

undersampling;

TF-IDF;

embeddings;

SHAP;

LIME;

PSI para drift;

validação cruzada;

clusterização;

centralidade em grafos;

busca semântica;

prompt zero-shot;

prompt few-shot;

classificação supervisionada;

classificação por LLM;

geração de mapas explicativos.

Em SemED-LLM, uma técnica pode ser a construção de prompts com exemplos. Em GeoReXAI, uma técnica pode ser a sobreposição de mapas de importância. Em FairED-Pipeline, uma técnica pode ser a mitigação por reamostragem.

### 5.5 Metodologia

Metodologia é a organização de métodos, etapas, procedimentos, papéis e critérios para conduzir uma pesquisa ou processo. Ela define como o trabalho será desenvolvido, aplicado e validado.

| Metodologia | Quando usar | Exemplo de projeto |

| --- | --- | --- |

| Design Science Research | Quando o trabalho cria e avalia um artefato | EdmLens, SemED-LLM, GeoReXAI |

| Action Design Research | Quando o artefato evolui com participação de usuários reais | MILA-eDU, UnespDataLens, SemED-LLM |

| Estudo de caso | Quando se demonstra a proposta em contexto real ou realista | EdmLens em dados educacionais, GeoReXAI em dados agrícolas |

| Pesquisa experimental | Quando se compara alternativas sob controle | FairED-Pipeline com e sem mitigação |

| Mapeamento sistemático | Quando se organiza o estado da arte | FairED-Pipeline |

| CRISP-DM | Quando o foco é mineração de dados | MILA-eDU, modelos de evasão |

| CRISP-ML(Q) | Quando há ciclo de vida de modelos de ML | EdmLens, GeoReXAI, FairED-Pipeline |

### 5.6 Arquitetura

Arquitetura é a organização estrutural de uma solução. Ela define componentes, módulos, relações, interfaces, fluxos, dependências, restrições e decisões de projeto.

Uma arquitetura responde:

Como a solução está organizada?

| Projeto | Arquitetura possível |

| --- | --- |

| EdmLens | Arquitetura modular para engenharia de dados educacionais |

| MILA-eDU | Arquitetura analítica para apoio à decisão educacional |

| UnespDataLens | Arquitetura de plataforma de conhecimento navegável |

| SemED-LLM | Arquitetura para diagnóstico semântico com LLMs |

| FairED-Pipeline | Arquitetura para auditoria de vieses em pipelines |

| GeoReXAI | Arquitetura geoespacial explicável |

| EduPipeX | Arquitetura para explicabilidade de pipelines |

Uma arquitetura pode ser validada por coerência estrutural, completude, separação de responsabilidades, aderência a requisitos, análise por especialistas, protótipo ou estudo de caso.

### 5.7 Pipeline

Pipeline é uma sequência operacional de etapas que transforma entradas em saídas. Em dados, um pipeline descreve como dados brutos são processados até se tornarem artefatos úteis.

| Projeto | Pipeline |

| --- | --- |

| EdmLens | Fontes → extração → transformação → integração → armazenamento → features → modelos → explicações → catálogo |

| SemED-LLM | Textos → anonimização → prompt → LLM → classificação → validação docente → relatório |

| FairED-Pipeline | Dataset → auditoria de grupos → métricas de fairness → mitigação → avaliação → documentação |

| GeoReXAI | Camadas geográficas → validação espacial → modelagem → explicabilidade → mapa interpretativo |

| EduPipeX | Dados → transformações → registros de decisão → explicações do pipeline → relatório |

| MILA-eDU | Dados educacionais → análise de fatores → priorização → decisão → avaliação |

O pipeline é mais operacional que a arquitetura. A arquitetura define a organização; o pipeline executa o fluxo.

### 5.8 Plataforma

Plataforma é um ambiente computacional integrado que oferece funcionalidades para usuários ou sistemas. Pode incluir interface, banco de dados, APIs, módulos, controle de acesso, visualizações, automações e mecanismos de execução.

| Projeto | Plataforma possível |

| --- | --- |

| UnespDataLens | Plataforma de navegação, estudo e descoberta de conceitos, métodos e projetos |

| EdmLens | Plataforma de documentação, execução e catálogo de pipelines educacionais |

| MILA-eDU | Plataforma de apoio à decisão educacional |

| SemED-LLM | Plataforma para análise semântica de interações estudantis |

| GeoReXAI | Plataforma para visualização geoespacial explicável |

| FairED-Pipeline | Plataforma de auditoria de vieses e fairness |

Uma plataforma deve ser validada não apenas por funcionamento técnico, mas também por usabilidade, utilidade, desempenho, segurança, adequação ao usuário e capacidade de apoiar tarefas reais.

### 5.9 Framework

Framework é uma estrutura organizada e reutilizável para tratar uma classe de problemas. Ele pode reunir conceitos, princípios, módulos, métodos, processos, arquitetura, artefatos, metadados, regras e critérios de avaliação.

Um framework responde:

Qual estrutura orienta a solução de uma classe de problemas?

| Projeto | Classe de problema |

| --- | --- |

| EdmLens | Engenharia de dados educacionais |

| MILA-eDU | Apoio analítico à decisão educacional |

| SemED-LLM | Diagnóstico semântico de interações estudantis |

| FairED-Pipeline | Auditoria e mitigação de vieses em pipelines educacionais |

| GeoReXAI | Modelagem geoespacial explicável |

| EduPipeX | Explicabilidade de pipelines de dados educacionais |

### 5.10 Framework técnico-metodológico

Framework técnico-metodológico é um framework que combina estrutura técnica e diretrizes metodológicas.

Ele é técnico porque define:

módulos;

entradas;

saídas;

artefatos;

metadados;

contratos;

logs;

modelos;

agentes;

parâmetros;

mecanismos computacionais;

exemplos de implementação.

Ele é metodológico porque define:

princípios;

etapas;

responsabilidades;

procedimentos;

critérios de avaliação;

documentação;

validação;

governança;

reprodutibilidade;

formas de aplicação;

formas de evolução.

Exemplos:

EdmLens pode ser definido como framework técnico-metodológico porque não apenas organiza módulos para engenharia de dados educacionais, mas também define artefatos, metadados, contratos, critérios, governança, proveniência, monitoramento, semântica, vieses, catálogo e documentação.

FairED-Pipeline pode ser um framework técnico-metodológico se, além das métricas de fairness, definir como identificar vieses, em que etapa, com quais dados, quais grupos, quais métricas, quais ações de mitigação, como documentar e como monitorar a evolução dos vieses.

SemED-LLM pode ser técnico-metodológico se, além de usar LLMs, formalizar prompts, taxonomias, critérios de validação, rastreabilidade, logs, limites de autonomia, governança e avaliação humana.

### 5.11 Artefato computacional

Artefato computacional é qualquer produto criado pela pesquisa para resolver, representar, automatizar, organizar ou avaliar um problema computacional.

Exemplos:

framework;

modelo;

método;

algoritmo;

arquitetura;

pipeline;

plataforma;

protótipo;

agente;

dataset;

catálogo;

ontologia;

glossário;

dashboard;

ferramenta;

biblioteca;

guia;

especificação;

repositório;

conjunto de templates.

Um artefato deve ser descrito, justificado, implementado ou instanciado, avaliado e documentado.

### 5.12 Fundamentação teórica e metodológica para propostas computacionais

Esta subseção complementa os conceitos fundamentais com referenciais metodológicos e arquiteturais que ajudam o aluno a justificar, construir, descrever, implementar e avaliar artefatos computacionais de forma científica.

A proposta de um framework precisa ser fundamentada teoricamente. Não basta dizer que uma arquitetura é útil; é necessário explicar que tipo de artefato está sendo produzido, em qual tradição metodológica ele se encaixa, como será descrito e como será avaliado.

### 3.1 Design Science Research - DSR

A DSR é indicada para pesquisas que constroem e avaliam artefatos destinados a resolver problemas relevantes. O artefato pode ser constructo, modelo, método, framework, arquitetura, algoritmo, protótipo ou sistema. Em projetos de Ciência da Computação aplicada, a DSR ajuda a justificar que a contribuição não é apenas empírica, mas também de projeto e construção de solução.

| Etapa DSR | Pergunta para o aluno | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- | --- |

| Problema | Que lacuna motiva o artefato? | Pipelines educacionais pouco rastreáveis. | LLMs sem validação docente. | Mapas preditivos sem explicabilidade. |

| Objetivos | O que o artefato deve resolver? | Governança e reprodutibilidade. | Diagnóstico semântico auditável. | XAI geoespacial. |

| Desenvolvimento | Como o artefato será construído? | Módulos e contratos. | Prompts e agentes. | Camadas espaciais e linhagem. |

| Demonstração | Onde será aplicado? | Dataset educacional. | Fóruns de AVA. | Dados de macronutrientes. |

| Avaliação | Como será julgado? | Qualidade e rastreabilidade. | F1 e validação humana. | Métricas + mapas + especialistas. |

### 3.2 Action Design Research - ADR

A ADR pode ser usada quando o artefato é construído em interação com o ambiente real e com os participantes do domínio. Ela é útil quando professores, gestores, especialistas ou usuários participam do refinamento do framework.

| Quando ADR é adequada | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- |

| Quando o artefato evolui com uso real. | Professor avalia diagnósticos gerados por LLM. | Gestor educacional ajusta indicadores do dashboard. | Especialista agrícola revisa explicações geoespaciais. |

| Quando a intervenção no contexto gera aprendizado. | Feedback docente altera taxonomia. | Uso do pipeline revela metadados necessários. | Usuários solicitam novas visões arquiteturais. |

| Quando pesquisa e prática se influenciam. | Protótipo muda a forma de analisar fóruns. | Framework muda rotinas de governança. | Agente monitorador altera ciclo de manutenção. |

### 3.3 Estudo de caso

O estudo de caso é adequado para demonstrar e avaliar um framework em um contexto real ou realista. Ele deve explicitar unidade de análise, contexto, dados, procedimento, fontes de evidência e limitações.

| Elemento | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- |

| Unidade de análise | Turma de Estruturas de Dados. | Curso de Ciência da Computação. | Talhão-safra ou região agrícola. |

| Fonte de evidência | Logs do AVA e notas. | Mensagens textuais e validação docente. | Dados geoespaciais e análises laboratoriais. |

| Resultado esperado | Pipeline executável e rastreável. | Diagnósticos semânticos avaliados. | Mapas explicativos e métricas espaciais. |

### 3.4 Pesquisa experimental

A pesquisa experimental é indicada quando o trabalho compara alternativas sob condições controladas. Em frameworks, pode-se comparar uma execução ad hoc com uma execução padronizada pelo framework, ou comparar modelos, métodos e configurações.

| Comparação | Variável independente | Variável dependente | Exemplo |

| --- | --- | --- | --- |

| Pipeline ad hoc vs. framework | Tipo de pipeline. | Cobertura de rastreabilidade e tempo de reexecução. | Avaliar se o framework melhora auditabilidade. |

| Modelos diferentes | Algoritmo ou LLM. | F1, acurácia, estabilidade, custo. | Comparar LLM, SVM e Random Forest. |

| Com e sem agente | Presença de agente inteligente. | Tempo de análise, erros, cobertura de logs. | Agente validador de qualidade. |

### 3.5 ISO/IEC/IEEE 42010 e descrição arquitetural

A descrição arquitetural deve identificar stakeholders, preocupações, visões, pontos de vista e modelos arquiteturais. Essa abordagem é importante para frameworks porque a mesma arquitetura precisa ser compreendida por pesquisadores, desenvolvedores, especialistas do domínio e avaliadores.

| Conceito | Definição operacional no guia | Três exemplos |

| --- | --- | --- |

| Stakeholder | Parte interessada na arquitetura. | Pesquisador; desenvolvedor; professor. |

| Concern | Preocupação relevante. | Reprodutibilidade; privacidade; escalabilidade. |

| Viewpoint | Convenção para construir uma visão. | Visão de dados; visão de processos; visão de implantação. |

| View | Representação concreta da arquitetura. | Diagrama de módulos; ER de metadados; fluxo de execução. |

### 3.6 CRISP-DM e CRISP-ML(Q)

CRISP-DM ajuda a organizar projetos de mineração de dados em fases, tarefas e saídas. CRISP-ML(Q) amplia essa perspectiva para aplicações de aprendizado de máquina com garantia de qualidade, monitoramento e manutenção.

| Fase | Exemplo educacional | Exemplo com LLM | Exemplo geoespacial |

| --- | --- | --- | --- |

| Compreensão do domínio | Entender evasão e desempenho. | Entender lacunas conceituais. | Entender fenômeno espacial. |

| Compreensão dos dados | Mapear notas, frequência e AVA. | Mapear textos e metadados. | Mapear camadas e atributos. |

| Preparação | Limpeza e integração. | Anonimização e prompts. | Tratamento espacial. |

| Modelagem | XGBoost, RF, regressão. | LLM, embeddings, classificadores. | RF espacial, GWR, redes. |

| Avaliação | AUC, F1, validação docente. | F1, consistência, análise humana. | RMSE, mapas, especialistas. |

| Monitoramento | Drift de dados educacionais. | Drift de prompts/respostas. | Mudança temporal/espacial. |

### 3.7 DataOps e MLOps

DataOps e MLOps fornecem fundamentos práticos para automação, versionamento, integração contínua, testes, monitoramento, colaboração e entrega confiável de produtos analíticos. Para o guia, esses referenciais ajudam a transformar a especificação em prática implementável.

| Prática | Aplicação 1 | Aplicação 2 | Aplicação 3 |

| --- | --- | --- | --- |

| Versionamento | Git para código. | DVC para dados. | MLflow para modelos. |

| Testes automatizados | Teste de schema. | Teste de qualidade. | Teste de agente. |

| Monitoramento | Drift de dados. | Queda de métrica. | Falha de agente. |

| Orquestração | Airflow. | Prefect. | Dagster. |

### 3.8 W3C PROV, FAIR e rastreabilidade

W3C PROV oferece uma base para representar proveniência por entidades, atividades e agentes. Os princípios FAIR orientam organização e reuso de dados e artefatos, com ênfase em serem encontráveis, acessíveis, interoperáveis e reutilizáveis.

| Princípio | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- |

| Findable | Dataset catalogado por ID. | Prompt versionado por nome. | Modelo registrado no catálogo. |

| Accessible | Acesso por política. | Metadados públicos. | Dados restritos com controle. |

| Interoperable | JSON/YAML/Parquet. | Vocabulários padronizados. | APIs documentadas. |

| Reusable | Licença e contexto. | Dicionário de dados. | Registro de qualidade. |

### 3.9 NIST AI RMF e governança de IA

Quando houver IA, LLMs ou agentes inteligentes, o framework deve tratar riscos, governança, monitoramento e responsabilização. A lógica Govern, Map, Measure e Manage pode ser adaptada para definir políticas, mapear riscos, medir comportamento e gerenciar incidentes.

| Função | Pergunta | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- | --- |

| Govern | Quem responde pela IA? | Docente valida diagnóstico. | Pesquisador aprova prompt. | Comitê avalia uso de dados. |

| Map | Quais riscos existem? | Viés contra grupos. | Alucinação do LLM. | Uso indevido de dado pessoal. |

| Measure | Como medir risco? | Concordância humana. | Taxa de erro por grupo. | Teste de robustez. |

| Manage | Como controlar risco? | Bloqueio de ação automática. | Revisão humana. | Registro de incidente. |

## 6. Da lacuna ao artefato

A robustez científica de uma proposta depende da relação entre lacuna, objetivo, artefato e avaliação.

Uma proposta deve evitar começar diretamente pelo desenho da solução. Antes disso, o pesquisador deve explicitar:

o problema observado;

a lacuna científica, técnica, metodológica ou arquitetural;

a classe de solução adequada;

o artefato proposto;

o modo de validação.

### 6.1 Formulação do problema

| Formulação fraca | Formulação forte | Por que melhora |

| --- | --- | --- |

| Há muitos dados educacionais | Instituições educacionais produzem dados heterogêneos que frequentemente são processados por pipelines ad hoc, pouco documentados e difíceis de reproduzir | Delimita o problema técnico |

| LLMs podem ajudar na educação | LLMs podem classificar interações textuais, mas sua aplicação educacional exige rastreabilidade de prompts, validação humana e governança | Inclui condições de uso |

| Modelos precisam ser explicáveis | Modelos geoespaciais podem produzir predições úteis, mas frequentemente não vinculam explicações aos dados, camadas e transformações que as originaram | Conecta explicabilidade à proveniência |

| É preciso apoiar decisões educacionais | Decisões sobre evasão e permanência exigem integração entre indicadores, análise, interpretação, priorização e avaliação de ações | Explicita processo decisório |

### 6.2 Tipos de lacuna

| Tipo de lacuna | Exemplo |

| --- | --- |

| Conceitual | Falta de definição clara entre método, técnica, metodologia, arquitetura e framework |

| Metodológica | Ausência de roteiro formal para conduzir análises educacionais orientadas à decisão |

| Técnica | Baixa automação de metadados, logs ou rastreabilidade |

| Arquitetural | Pouca integração entre módulos de dados, governança e modelagem |

| Avaliativa | Ausência de métricas para avaliar aderência, rastreabilidade ou reprodutibilidade |

| Semântica | Conceitos e variáveis educacionais pouco documentados |

| Ética/governança | Uso de dados sensíveis sem controle, registro ou finalidade explícita |

| Reprodutibilidade | Dificuldade de reconstruir experimentos, modelos, prompts ou pipelines |

### 6.3 Transformação da lacuna em objetivo

| Lacuna | Objetivo geral correspondente | Artefato esperado |

| --- | --- | --- |

| Pipelines educacionais ad hoc | Propor e avaliar um framework modular para pipelines educacionais rastreáveis e reprodutíveis | EdmLens |

| Decisões educacionais pouco sistematizadas | Propor metodologia analítica para apoiar decisões educacionais baseadas em evidências | MILA-eDU |

| Conceitos dispersos em dados e IA | Propor plataforma de conhecimento para organizar conceitos, métodos e exemplos | UnespDataLens |

| LLMs sem governança no diagnóstico educacional | Propor framework para diagnóstico semântico com LLMs, validação docente e rastreabilidade | SemED-LLM |

| Modelos com risco de viés | Propor framework para identificação, mensuração e mitigação de vieses em pipelines educacionais | FairED-Pipeline |

| Predições geoespaciais pouco explicáveis | Propor framework geoespacial explicável com proveniência dos dados e mapas | GeoReXAI |

| Pipelines pouco explicáveis | Propor framework para explicabilidade de transformações e decisões em pipelines | EduPipeX |

### 6.4 Questões de pesquisa

As questões de pesquisa devem explicitar o que será investigado, demonstrado ou avaliado na proposta. Elas podem ter caráter estrutural, técnico, avaliativo, metodológico ou aplicado.

| Tipo de RQ | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- |

| Estrutural | Como organizar módulos para integrar governança e modelagem? | Como estruturar agentes em pipeline educacional? | Como organizar XAI em pipeline geoespacial? |

| Operacional | Como contratos e metadados permitem execução reprodutível? | Como prompts versionados afetam consistência? | Como camadas geográficas podem ser rastreadas? |

| Avaliativa | Qual a cobertura de linhagem obtida? | Qual a concordância entre agente e docente? | Especialistas consideram mapas explicáveis úteis? |

## 7. Estrutura recomendada para formalização de propostas

Este guia recomenda organizar propostas computacionais em quatro níveis principais.

| Nível | Função |

| --- | --- |

| Proposta principal | Define o tipo de contribuição: framework, plataforma, método, modelo, arquitetura etc. |

| Modelo de referência ou fundamentação estrutural | Formaliza elementos conceituais essenciais |

| Arquitetura ou organização funcional | Mostra componentes, módulos, fluxos e relações |

| Especificação técnico-metodológica | Detalha módulos, artefatos, metadados, contratos, avaliação e implementação |

Nem toda proposta precisa ter todos os níveis com a mesma profundidade. Um método pode não exigir uma arquitetura modular complexa. Uma plataforma pode exigir mais descrição de usuários, funcionalidades e requisitos. Um framework técnico-metodológico exige os quatro níveis de forma mais completa.

## 8. Modelo de referência para propostas computacionais

Um modelo de referência pode ser formalizado como:

MR = {P, C, A, MD, CT, R, Q, D}

Em que:

P representa princípios;

C representa componentes ou módulos;

A representa artefatos;

MD representa metadados;

CT representa contratos;

R representa relações;

Q representa critérios de qualidade e avaliação;

D representa dimensões transversais.

### 8.1 Exemplo aplicado a diferentes projetos

| Elemento | EdmLens | MILA-eDU | UnespDataLens | SemED-LLM | FairED-Pipeline | GeoReXAI |

| --- | --- | --- | --- | --- | --- | --- |

| P | Governança, rastreabilidade, reprodutibilidade | Decisão orientada por evidência | Navegação e aprendizagem | Validação semântica | Justiça e auditoria | Explicabilidade espacial |

| C | Módulos de pipeline | Etapas analíticas | Módulos de conhecimento | Ingestão, prompt, validação | Auditoria, métrica, mitigação | Camadas, modelo, XAI |

| A | Datasets, features, modelos | Indicadores, cenários, recomendações | Páginas, conceitos, links | Classificações, logs, prompts | Relatórios de viés | Mapas, camadas, explicações |

| MD | Técnicos, semânticos, governança | Indicadores e decisões | Conceitos e relações | Prompt, modelo, resposta | Grupos, métricas, limiares | CRS, camada, resolução |

| CT | Contratos de módulo | Critérios de decisão | Padrões de página | Contrato de resposta LLM | Contrato de fairness | Contrato geoespacial |

| R | Linhagem | Relação fator-decisão | Relação conceito-módulo | Texto-prompt-classe | Grupo-métrica-mitigação | Camada-predição-mapa |

| Q | Qualidade, drift, catálogo | Utilidade decisória | Clareza e navegabilidade | Concordância docente | Paridade, erro por grupo | RMSE, utilidade do mapa |

| D | Privacidade, semântica, fairness | Associação, causalidade, impacto | Semântica, reuso | Governança de IA | Fairness transversal | XAI e proveniência |

## 9. Descrição arquitetural da proposta

A arquitetura deve ser descrita por múltiplas visões. Uma única figura raramente é suficiente.

### 9.1 Visão conceitual

Representa conceitos do domínio e suas relações.

Exemplos:

EdmLens: fonte, dataset, feature, modelo, explicação, catálogo.

MILA-eDU: estudante, fator, indicador, risco, ação, impacto.

SemED-LLM: interação, conceito, lacuna, taxonomia, diagnóstico.

UnespDataLens: conceito, módulo, técnica, método, exemplo, link.

GeoReXAI: camada, região, atributo, predição, explicação.

FairED-Pipeline: grupo, métrica, viés, mitigação, decisão.

### 9.2 Visão lógica

Representa módulos e responsabilidades.

Exemplos:

ingestão;

transformação;

integração;

modelagem;

explicabilidade;

governança;

validação humana;

catálogo;

monitoramento;

mitigação;

recomendação;

visualização.

### 9.3 Visão de dados

Representa entidades, schemas, metadados e formatos.

Exemplos:

tabela de estudantes;

registro de prompt;

feature set;

camada geográfica;

relatório de fairness;

dicionário de conceitos.

### 9.4 Visão de processo

Representa fluxos e execução.

Exemplos:

pipeline de dados;

workflow de validação;

ciclo de análise;

fluxo de decisão;

ciclo de monitoramento;

processo de reavaliação.

### 9.5 Visão de implementação

Representa tecnologias, repositórios, APIs, scripts, bancos, serviços e estrutura de código.

Exemplos:

Python + PostgreSQL;

FastAPI + LLM;

GeoPandas + PostGIS;

GitHub Pages + Markdown;

MLflow + DVC;

Airflow, Prefect ou Dagster.

### 9.6 Visão de governança

Representa papéis, políticas, restrições, segurança e responsabilidades.

Exemplos:

quem pode acessar;

quem valida;

quem aprova;

quais dados são restritos;

quais ações são bloqueadas;

como registrar logs;

como auditar.

### 9.7 Visão de proveniência

Representa linhagem entre dados, processos, agentes, modelos, explicações e resultados.

Exemplos:

dataset → feature → modelo → explicação → relatório;

texto → prompt → resposta → validação → diagnóstico;

camada geográfica → modelo → mapa → interpretação;

grupo → métrica de fairness → mitigação → nova avaliação.

### 9.8 Descrição arquitetural sintética e decisões arquiteturais

Além das visões arquiteturais, recomenda-se registrar uma descrição sintética da arquitetura e suas decisões de projeto, indicando justificativas, alternativas consideradas e impactos esperados.

Uma arquitetura de framework deve ser descrita por múltiplas visões. Cada visão atende a uma preocupação diferente e evita que a proposta seja reduzida a uma única figura genérica.

| Visão | O que representa | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- | --- |

| Conceitual | Conceitos e relações do domínio. | Estudante-interação-lacuna. | Fonte-dataset-feature. | Camada-região-predição. |

| Lógica | Módulos e responsabilidades. | Ingestão, transformação, modelagem. | Prompt, agente, validação. | Pré-processamento, mapa, XAI. |

| Dados | Entidades, schemas e metadados. | Tabela estudante. | Registro de prompt. | Tabela camada geográfica. |

| Processo | Fluxo de execução. | Pipeline educacional. | Workflow LLM. | Workflow espacial. |

| Implementação | Tecnologias e estrutura de código. | Python + PostgreSQL. | FastAPI + LLM. | GeoPandas + PostGIS. |

| Governança | Papéis, políticas e restrições. | Anonimização. | Validação humana. | Permissão por projeto. |

| Proveniência | Linhagem de dados e artefatos. | dataset→modelo→relatório. | texto→prompt→classe. | shape→modelo→mapa. |

### 5.1 Exemplo de descrição arquitetural sintética

A arquitetura proposta é organizada em módulos funcionais e módulos transversais. Os módulos funcionais executam o fluxo principal de processamento dos dados, enquanto os módulos transversais registram governança, qualidade, proveniência, monitoramento e reprodutibilidade. Essa separação permite que o framework seja implementado como pipeline operacional, mas também auditado como artefato científico.

### 5.2 Decisões arquiteturais

| Decisão | Justificativa | Trade-off |

| --- | --- | --- |

| Usar arquivos Parquet na camada processada. | Eficiência e preservação de schema. | Exige bibliotecas específicas. |

| Registrar logs em JSON. | Facilita integração e auditoria. | Pode gerar volume elevado de registros. |

| Exigir validação humana em agentes de decisão. | Reduz risco em domínio sensível. | Aumenta tempo de operação. |

| Separar governança como módulo transversal. | Garante políticas em todo pipeline. | Exige maior disciplina de implementação. |

## 10. Especificação formal de módulos ou componentes

Cada módulo deve ter especificação padronizada.

| Campo | O que deve conter |

| --- | --- |

| Nome | Identificação formal |

| Tipo | Operacional, analítico, transversal, especializado |

| Finalidade | Por que existe |

| Objetivo | O que pretende realizar |

| Problema tratado | Lacuna que resolve |

| Responsabilidades | O que faz |

| Fora do escopo | O que não faz |

| Entradas | Dados, parâmetros, artefatos, metadados |

| Processamento | Operações internas |

| Saídas | Produtos gerados |

| Artefatos | Itens formais produzidos |

| Metadados | Registros necessários |

| Contratos | Entrada, saída, qualidade, erro |

| Governança | Políticas e restrições |

| Qualidade | Critérios mínimos |

| Estados | Ativo, pendente, bloqueado, obsoleto |

| Erros | Falhas previstas |

| Métricas | Indicadores de avaliação |

| Relações | Dependências com outros módulos |

| Exemplos | Cenários de uso |

| Implementação | Código, JSON, YAML, pseudocódigo ou diretórios |

### 10.1 Templates e exemplos de especificação formal de módulos

A especificação de módulos deve ser operacional, permitindo que o aluno identifique entradas, saídas, artefatos, metadados, contratos, métricas e evidências de execução.

Cada módulo deve ser descrito de modo uniforme. O objetivo é permitir que o aluno transforme a especificação em implementação. Uma descrição apenas textual é insuficiente; é necessário declarar entradas, saídas, contratos, artefatos, metadados, erros e critérios de avaliação.

### 6.1 Template obrigatório do módulo

| Campo | O que escrever | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- | --- |

| Objetivo | Finalidade central. | Ingerir dados. | Classificar textos. | Gerar mapas explicativos. |

| Responsabilidade | O que faz. | Valida schema. | Executa prompt. | Calcula SHAP espacial. |

| Fora do escopo | O que não faz. | Não treina modelo. | Não atribui nota. | Não altera coordenadas. |

| Entradas | Dados necessários. | CSV, schema, política. | Texto, contexto, prompt. | Shape, variáveis, modelo. |

| Saídas | Produtos gerados. | Dataset validado. | Classe e explicação. | Mapa e relatório. |

| Metadados | Registros sobre execução. | ID, fonte, versão. | Prompt, modelo, temperatura. | CRS, camada, resolução. |

| Qualidade | Critérios mínimos. | Completude > 95%. | Concordância > 0,75. | Sem geometria inválida. |

| Avaliação | Como julgar. | Teste de ingestão. | Validação docente. | Avaliação por especialista. |

### 6.2 Exemplo 1: módulo de ingestão

Objetivo: receber dados brutos de fontes autorizadas, validar estrutura mínima, registrar metadados iniciais e armazenar uma versão imutável dos dados.

| Elemento | Especificação |

| --- | --- |

| Entradas | dataset_bruto, schema_esperado, identificador_fonte, política_acesso, responsável. |

| Processamento | Validar formato, campos obrigatórios, calcular hash, registrar origem, armazenar raw. |

| Saídas | dataset_raw_versionado, log_ingestao, metadados_fonte, relatório de validação. |

| Metadados | id_execucao, id_fonte, data, versão, hash, número de registros, status. |

| Critérios | 100% dos campos obrigatórios presentes; origem registrada; hash calculado. |

### 6.3 Exemplo 2: módulo de classificação semântica com LLM

Objetivo: classificar interações textuais segundo uma taxonomia de categorias ou lacunas conceituais, registrando prompt, modelo, parâmetros e justificativa.

| Elemento | Especificação |

| --- | --- |

| Entradas | texto_anonimizado, contexto_disciplina, taxonomia, prompt_versionado, parâmetros_llm. |

| Processamento | Montar prompt, chamar modelo, validar formato da resposta, registrar saída. |

| Saídas | classe_semantica, lacuna, confiança, explicação, log_agente. |

| Metadados | versão_prompt, modelo, temperatura, data, id_interacao, status_validação. |

| Critérios | Resposta aderente à taxonomia; validação humana em amostra; registro completo. |

### 6.4 Exemplo 3: módulo de explicabilidade

Objetivo: gerar explicações associadas aos resultados de modelos ou agentes, preservando vínculo com dados, modelo, método explicativo e contexto.

| Elemento | Especificação |

| --- | --- |

| Entradas | modelo_treinado, dataset_features, método_explicativo, instâncias selecionadas. |

| Processamento | Calcular explicações locais/globais, validar consistência, gerar relatório. |

| Saídas | explicações, ranking de variáveis, gráficos, relatório interpretativo. |

| Metadados | id_modelo, id_dataset, método, versão_biblioteca, parâmetros. |

| Critérios | Explicações vinculadas ao modelo; gráficos legíveis; interpretação validada. |

## 11. Artefatos e metadados

Todo artefato deve ter identidade, versão, origem, responsável, localização, qualidade, restrição de uso e relação com outros artefatos.

### 11.1 Exemplos de artefatos por projeto

| Projeto | Artefatos |

| --- | --- |

| EdmLens | Datasets, features, modelos, explicações, logs, catálogo |

| MILA-eDU | Indicadores, cenários, recomendações, relatórios de decisão |

| UnespDataLens | Páginas, glossário, mapas conceituais, links, módulos |

| SemED-LLM | Prompts, respostas, classificações, validações, diagnósticos |

| FairED-Pipeline | Métricas de fairness, relatórios de viés, ações de mitigação |

| GeoReXAI | Mapas, camadas, modelos, explicações espaciais |

| EduPipeX | Registros de transformação, explicações de pipeline, relatórios |

### 11.2 Categorias de metadados

| Categoria | Exemplos |

| --- | --- |

| Descritivos | nome, descrição, domínio, responsável |

| Técnicos | formato, schema, versão, localização |

| Semânticos | significado, unidade de análise, categoria, conceito |

| Operacionais | data, ambiente, execução, script |

| Qualidade | completude, consistência, validade |

| Governança | sensibilidade, acesso, finalidade, restrição |

| Proveniência | origem, atividade, agente, derivação |

| Monitoramento | status, drift, alerta, validade |

| Catálogo | tags, palavras-chave, status, reuso |

| Agentes | prompt, modelo, autonomia, validação humana |

### 11.3 Exemplos detalhados de metadados por domínio

Os metadados devem ser adaptados ao tipo de proposta, ao domínio e aos artefatos produzidos. A seguir são incorporados exemplos para dados educacionais, LLMs/agentes e dados geoespaciais.

Metadados são dados sobre dados, processos, modelos, agentes e artefatos. Eles são essenciais para organização, governança, reuso, auditoria e reprodutibilidade.

### 8.1 Tipos de metadados

| Tipo | Pergunta que responde | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- | --- |

| Descritivo | O que é este ativo? | Nome do dataset. | Descrição do prompt. | Título do relatório. |

| Estrutural | Como está organizado? | Campos e tipos. | Formato da resposta. | Sistema de coordenadas. |

| Administrativo | Quem gerencia? | Responsável. | Permissão. | Política de retenção. |

| Qualidade | É confiável? | Completude. | Consistência. | Acurácia. |

| Proveniência | De onde veio? | Fonte. | Derivação. | Agente responsável. |

| Técnico | Como foi gerado? | Commit. | Docker image. | Parâmetros. |

| Ético/legal | Pode ser usado? | Consentimento. | Anonimização. | Restrição de acesso. |

| Agente | Como o agente atuou? | Prompt. | Modelo. | Nível de autonomia. |

### 8.2 Três exemplos de metadados

Exemplo de metadados de dataset:

{

"id_dataset": "interacoes_forum_v1",

"fonte": "Moodle",

"periodo": "2025-01-01/2025-12-31",

"formato": "parquet",

"registros": 15432,

"responsavel": "pesquisador_01",

"restricao": "anonimizado",

"versao": "1.0"

}

Exemplo de metadados de modelo:

{

"id_modelo": "evasao_xgb_v4",

"algoritmo": "XGBoost",

"dataset_treinamento": "features_v3",

"metricas": {"auc": 0.91, "f1": 0.84},

"hiperparametros": {"max_depth": 5, "learning_rate": 0.05},

"seed": 42,

"commit": "abc123"

}

Exemplo de metadados de prompt/agente:

{

"id_prompt": "prompt_lacunas_v3",

"agente": "agente_diagnostico_semantico",

"modelo_base": "LLM",

"temperatura": 0.0,

"taxonomia": "taxonomia_lacunas_v2",

"requer_validacao_humana": true,

"restricoes": ["nao_atribuir_nota", "nao_expor_dados_pessoais"]

}

## 12. Contratos

Contratos tornam uma proposta implementável e avaliável. Eles definem o que cada módulo, método, agente, pipeline ou artefato exige, produz e garante.

### 12.1 Tipos de contratos

| Tipo | Define | Exemplo |

| --- | --- | --- |

| Entrada | O que o módulo aceita | dataset, texto, prompt, camada |

| Saída | O que o módulo produz | feature, classe, mapa, relatório |

| Qualidade | Critérios mínimos | completude, concordância, RMSE |

| Erro | Falhas e tratamentos | schema inválido, prompt fora do formato |

| Execução | Pré e pós-condições | fonte autorizada, modelo carregado |

| Governança | Restrições | dado anonimizado, validação humana |

### 12.2 Exemplo de contrato genérico

{

"modulo": "M_Transformacao",

"versao": "1.0",

"entrada": {

"artefato_entrada": {"obrigatorio": true},

"schema": {"obrigatorio": true},

"regras": {"obrigatorio": true}

},

"saida": {

"artefato_saida": "obrigatorio",

"log_execucao": "obrigatorio",

"metadados": "obrigatorio",

"registro_proveniencia": "obrigatorio"

},

"qualidade_minima": {

"completude": 0.95,

"rastreabilidade": true,

"governanca_validada": true

},

"erros_criticos": [

"schema_invalido",

"dados_sensiveis_sem_politica",

"ausencia_de_metadados"

]

}



### 12.3 Exemplos de contratos por domínio

Contratos devem tornar explícitas as obrigações de entrada, saída, qualidade, erro e governança entre módulos. Eles também podem ser adaptados a pipelines de dados, LLMs, agentes e análise geoespacial.

### 7.3 Três exemplos de contrato por domínio

| Domínio | Entrada obrigatória | Saída obrigatória | Erro crítico |

| --- | --- | --- | --- |

| Educação | id_estudante_anonimizado, disciplina, atividade, data. | dataset educacional validado. | dado pessoal não anonimizado. |

| LLM educacional | texto, taxonomia, prompt versionado. | classe, explicação, log de prompt. | resposta fora da taxonomia. |

| Geoespacial | geometria válida, CRS, atributos. | camada processada e mapa. | geometria inválida sem correção. |

## 13. Dimensões transversais

Algumas dimensões não pertencem a apenas um módulo. Elas atravessam toda a proposta.

### 13.1 Governança

Define papéis, políticas, responsabilidades, acesso, finalidade, retenção, descarte, validação, bloqueios e auditoria.

### 13.2 Qualidade

Avalia completude, consistência, validade, unicidade, integridade, atualidade, coerência semântica e confiabilidade.

### 13.3 Proveniência e linhagem

Registra origem, atividades, agentes, transformações, dependências, versões e derivação dos artefatos.

### 13.4 Semântica

Documenta o significado dos dados, categorias, conceitos, indicadores, features, prompts, classes, mapas ou recomendações.

### 13.5 Vieses e fairness

Avalia riscos de cobertura, seleção, ausência de dados, representação, modelagem, explicabilidade e uso.

### 13.6 Privacidade e segurança

Trata anonimização, pseudonimização, controle de acesso, criptografia, logs, minimização e proteção contra uso indevido.

### 13.7 Explicabilidade

Explica modelos, transformações, agentes, decisões, recomendações, mapas, relatórios e limitações.

### 13.8 Monitoramento e drift

Acompanha mudanças em dados, schema, features, modelos, prompts, explicações, mapas, indicadores ou desempenho.

### 13.9 Reprodutibilidade

Registra dados, código, ambiente, parâmetros, versões, seeds, prompts, modelos, logs e dependências.

### 13.10 Catálogo e reuso

Organiza descoberta, documentação, tags, status, restrições, versionamento e reutilização dos artefatos.

### 13.11 Rastreabilidade, governança, qualidade, ética, segurança e reprodutibilidade

As dimensões transversais precisam ser operacionalizadas por registros, papéis, políticas, métricas, logs, versionamento e mecanismos de auditoria.

## 9. Rastreabilidade, proveniência e linhagem

Rastreabilidade é a capacidade de reconstruir o caminho entre dados de entrada, processos, artefatos intermediários, modelos, explicações, decisões e resultados finais. Ela é essencial para confiabilidade científica, reprodutibilidade e auditoria.

### 9.1 O que rastrear

| Objeto | Pergunta | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- | --- |

| Dado | De onde veio? | Moodle. | Arquivo CSV. | Camada geográfica. |

| Processo | O que foi feito? | Limpeza. | Prompting. | Interpolação espacial. |

| Modelo | Como foi treinado? | Features v3. | Prompt v2. | Parâmetros espaciais. |

| Explicação | O que justificou? | SHAP. | Justificativa textual. | Mapa de importância. |

| Decisão | O que foi recomendado? | Intervenção. | Revisão de conceito. | Ação em área crítica. |

| Agente | Quem/que executou? | Script. | LLM agent. | Orquestrador. |

### 9.2 Três exemplos de linhagem

# Exemplo educacional

dataset_moodle_raw_v1 -> limpeza_v1 -> dataset_limpo_v1 -> features_v1 -> modelo_evasao_v1 -> relatorio_turma_v1

# Exemplo com LLM

texto_original -> texto_anonimizado -> prompt_lacunas_v3 -> resposta_llm -> classificacao_validada -> diagnostico_docente

# Exemplo geoespacial

shape_talhoes_v1 -> validacao_geometria -> integracao_solo_foliar -> modelo_predicao -> shap_espacial -> mapa_explicativo

### 9.3 Registro de proveniência

{

"entidade_gerada": "relatorio_turma_A_v1",

"foi_derivada_de": ["features_v3", "modelo_evasao_v4", "explicacoes_shap_v2"],

"atividade": "geracao_relatorio",

"agente": "script_relatorio.py",

"parametros": {"turma": "A", "periodo": "2025"},

"timestamp": "2026-06-11T10:30:00"

}

### 9.4 Consultas que o framework deve responder

Qual dado originou este resultado?

Quais transformações foram aplicadas?

Qual agente ou script executou a transformação?

Qual versão do código, prompt ou modelo foi usada?

Quais parâmetros foram utilizados?

Qual explicação fundamentou a decisão?

Quem validou a recomendação?

O resultado pode ser reproduzido?

Há registros suficientes para auditoria?

Que artefatos foram derivados deste dado?

## 10. Governança, qualidade, ética e segurança

Governança define papéis, responsabilidades, políticas e controles. Em frameworks acadêmicos, governança não deve ser vista como burocracia, mas como mecanismo de confiabilidade científica e proteção de indivíduos afetados.

### 10.1 Papéis e responsabilidades

| Papel | Responsabilidade | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- | --- |

| Pesquisador responsável | Responder pelo protocolo e avaliação. | Aprova dados. | Valida resultados. | Assina relatório. |

| Desenvolvedor | Implementar módulos e testes. | Cria ETL. | Cria API. | Automatiza logs. |

| Especialista do domínio | Validar significado. | Professor. | Agrônomo. | Gestor público. |

| Administrador de dados | Controlar acesso. | Permissões. | Backup. | Retenção. |

| Agente inteligente | Executar tarefa delimitada. | Classificar. | Monitorar. | Recomendar. |

### 10.2 Qualidade de dados

| Dimensão | Definição | Exemplo de métrica | Exemplo de ação |

| --- | --- | --- | --- |

| Completude | Ausência de valores faltantes. | % de campos preenchidos. | Imputar ou bloquear. |

| Consistência | Ausência de contradições. | Violações de regra. | Corrigir ou relatar. |

| Validade | Conformidade com domínio/tipo. | % de campos válidos. | Converter ou rejeitar. |

| Unicidade | Ausência de duplicidade. | Taxa de duplicados. | Remover duplicados. |

| Atualidade | Dados temporalmente adequados. | Idade do dado. | Atualizar fonte. |

| Integridade | Relações preservadas. | Chaves inválidas. | Corrigir relacionamento. |

### 10.3 Políticas mínimas

politica_governanca:

acesso:

dados_identificados: restrito

dados_anonimizados: pesquisadores_autorizados

resultados_agregados: professores_e_gestores

privacidade:

anonimizar_identificadores: true

remover_textos_sensiveis: true

agentes:

exigir_log: true

exigir_validacao_humana_para_alto_impacto: true

bloquear_acoes_nao_autorizadas: true

auditoria:

manter_logs: true

manter_linhagem: true

manter_versoes: true

## 11. Reprodutibilidade

Reprodutibilidade é a capacidade de executar novamente o pipeline, nas mesmas condições ou em condições equivalentes, obtendo resultados compatíveis. Ela exige controle de dados, código, ambiente, parâmetros, sementes, modelos, prompts e artefatos.

### 11.1 O que versionar

| Elemento | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- |

| Código | Git commit. | Tag de release. | Branch experimental. |

| Dados | DVC. | Data lake versionado. | Hash de arquivo. |

| Ambiente | Dockerfile. | Conda env. | requirements.txt. |

| Modelos | MLflow. | Arquivo pickle. | Registro de modelo. |

| Prompts | prompt_v1.txt. | YAML com instruções. | Registro no catálogo. |

| Resultados | Métricas JSON. | Relatórios HTML. | Logs de execução. |

### 11.2 Configuração reprodutível

experimento:

id: exp_001

seed: 42

data: 2026-06-11

ambiente:

python: "3.11"

docker_image: "framework:v1"

dados:

dataset: "interacoes_forum"

versao: "v2"

pipeline:

modulos: [ingestao, transformacao, classificacao, explicabilidade, relatorio]

modelo:

tipo: "llm"

prompt: "prompt_lacunas_v3"

temperatura: 0.0

rastreabilidade:

salvar_logs: true

salvar_linhagem: true

salvar_prompts: true

### 11.3 Três níveis de reprodutibilidade

| Nível | Descrição | Exemplo |

| --- | --- | --- |

| Mínimo | Documenta dados, código e parâmetros. | README com instruções e requirements. |

| Intermediário | Versiona dados, modelos e logs. | Git + DVC + MLflow. |

| Avançado | Ambiente conteinerizado e pipeline orquestrado. | Docker + Prefect + testes automatizados. |

## 14. Agentes inteligentes

Agentes inteligentes devem ser tratados como componentes arquiteturais especializados, e não como caixas genéricas de IA.

### 14.1 O que especificar em um agente

| Campo | Descrição |

| --- | --- |

| Nome | Identificação do agente |

| Objetivo | Tarefa principal |

| Entradas | Dados, contexto, prompt, regras |

| Saídas | Classificação, alerta, recomendação, explicação |

| Autonomia | Nível de decisão permitido |

| Restrições | O que não pode fazer |

| Rastreabilidade | Logs, prompts, respostas, versões |

| Governança | Validação humana, limites, bloqueios |

| Avaliação | Métricas, concordância, utilidade, erros |

### 14.2 Exemplos

| Projeto | Agente possível |

| --- | --- |

| SemED-LLM | Agente de diagnóstico semântico |

| EdmLens | Agente monitorador de drift |

| FairED-Pipeline | Agente auditor de fairness |

| UnespDataLens | Agente de navegação conceitual |

| MILA-eDU | Agente de apoio à priorização de ações |

| GeoReXAI | Agente explicativo de mapas |

| EduPipeX | Agente explicador de transformações |

### 14.3 Especificação ampliada de agentes inteligentes

Quando houver agentes inteligentes, o guia deve explicitar tipos de agentes, níveis de autonomia, templates de especificação, exemplos completos e registros de ação.

Agentes inteligentes devem ser tratados como componentes arquiteturais especializados. Eles não devem aparecer apenas como “IA” dentro da figura. Cada agente precisa ter objetivo, entradas, saídas, autonomia, restrições, logs, explicabilidade, governança e avaliação.

### 12.1 Tipos de agentes

| Tipo | Função | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- | --- |

| Validador | Verifica qualidade/conformidade. | Schema. | Anonimização. | Formato de resposta. |

| Classificador | Atribui categorias. | Lacuna conceitual. | Tipo de erro. | Classe de risco. |

| Explicativo | Gera justificativas. | SHAP textual. | Explicação docente. | Resumo de variáveis. |

| Recomendador | Sugere ações. | Revisar conteúdo. | Intervenção pedagógica. | Coleta adicional. |

| Monitorador | Observa mudanças. | Drift. | Falha de API. | Queda de métrica. |

| Orquestrador | Coordena módulos. | Reexecuta etapa. | Aciona validação. | Agenda pipeline. |

### 12.2 Níveis de autonomia

| Nível | Descrição | Exemplo seguro |

| --- | --- | --- |

| 0 | Sem agente; execução fixa. | Script executado manualmente. |

| 1 | Agente analisa e registra. | Detecta inconsistência e gera alerta. |

| 2 | Agente recomenda, mas não executa. | Sugere intervenção ao professor. |

| 3 | Executa com validação humana. | Gera relatório que precisa de aprovação. |

| 4 | Executa ações automáticas de baixo risco. | Atualiza dashboard de métricas. |

| 5 | Autonomia ampla com supervisão posterior. | Orquestra workflows adaptativos. |

### 12.3 Template de especificação de agente

| Campo | Descrição | Exemplo |

| --- | --- | --- |

| Nome | Identificação do agente. | Agente de Diagnóstico Semântico. |

| Objetivo | Tarefa principal. | Classificar lacunas conceituais. |

| Entradas | Dados e contexto. | Texto, disciplina, taxonomia, prompt. |

| Saídas | Artefatos gerados. | Classe, explicação, recomendação, log. |

| Autonomia | Nível permitido. | Nível 2: recomenda, não executa. |

| Restrições | O que não pode fazer. | Não atribuir nota; não expor dados. |

| Rastreabilidade | O que registrar. | Prompt, modelo, resposta, validação. |

| Avaliação | Como medir. | F1, concordância docente, auditoria. |

### 12.4 Três exemplos de agentes completos

| Agente | Entradas | Saídas | Avaliação |

| --- | --- | --- | --- |

| Agente de Diagnóstico Semântico | Texto, taxonomia, prompt, contexto. | Lacuna, explicação, recomendação. | F1, concordância docente, utilidade. |

| Agente Validador de Qualidade | Dataset, schema, regras. | Relatório de qualidade, alertas. | Taxa de detecção, cobertura de regras. |

| Agente Monitorador de Drift | Métricas temporais, features, modelos. | Alerta de drift, relatório. | Detecção de mudança, falso positivo. |

### 12.5 Registro de ação de agente

{

"id_acao": "acao_001",

"agente": "Agente_Diagnostico_Semantico",

"nivel_autonomia": 2,

"entrada": {"id_interacao": "int_38921", "texto": "Não entendi pilha e fila"},

"saida": {"classe": "duvida_conceitual", "lacuna": "pilha_vs_fila", "confianca": 0.82},

"modelo": "llm_x",

"prompt": "prompt_lacunas_v3",

"validacao_humana": true,

"status": "pendente_validacao"

}

## 15. Validação e avaliação da proposta

A validação e a avaliação constituem etapas centrais na formalização de propostas acadêmicas em Ciência da Computação. Uma proposta não se torna cientificamente robusta apenas por apresentar uma arquitetura, um framework, uma metodologia, um método, uma plataforma, um pipeline, um modelo, um agente inteligente ou um artefato computacional. É necessário demonstrar, por meio de evidências, que a proposta é coerente, aplicável, útil, tecnicamente viável, metodologicamente adequada, avaliável e compatível com a lacuna de pesquisa que motivou sua criação.

Neste guia, a validação deve ser compreendida como o processo de demonstrar que a proposta atende ao problema para o qual foi concebida. A avaliação corresponde ao processo de julgar a proposta com base em critérios explícitos, métricas, instrumentos e evidências. A verificação, por sua vez, consiste em confirmar se o artefato foi construído corretamente, de acordo com sua especificação.

| Conceito | Pergunta central | Exemplo |

| --- | --- | --- |

| Verificação | O artefato foi construído corretamente? | O módulo executa? O contrato foi respeitado? O código gera a saída esperada? |

| Validação | O artefato atende ao problema e ao contexto? | O framework ajuda a estruturar pipelines mais rastreáveis? |

| Avaliação | Qual é a qualidade, desempenho, utilidade ou aderência do artefato? | Qual a cobertura de metadados? Qual o F1 do agente? Qual a satisfação dos usuários? |

Uma validação adequada não deve ser descrita apenas por expressões genéricas, como “será validada por especialistas”, “será aplicada em um estudo de caso” ou “será avaliada por métricas”. É necessário detalhar como a validação será conduzida: quais etapas serão executadas, quais critérios serão utilizados, quais métricas serão calculadas, quais instrumentos serão aplicados, quais evidências serão coletadas, quem participará, como os resultados serão analisados e quais limitações serão consideradas.

Cada tipo de proposta exige um delineamento próprio. Um modelo conceitual não deve ser validado da mesma forma que uma plataforma. Uma metodologia não deve ser avaliada apenas por acurácia de modelo. Uma arquitetura não deve ser julgada apenas por parecer subjetivo. Um agente inteligente não deve ser avaliado apenas por utilidade percebida, mas também por precisão, segurança, rastreabilidade e controle de autonomia. Um framework técnico-metodológico exige avaliação multicritério, pois combina estrutura técnica, orientação metodológica, artefatos, metadados, contratos, governança e reprodutibilidade.

### 15.1 Protocolo geral de validação

A validação de qualquer proposta deve seguir um protocolo explícito. Esse protocolo funciona como um plano de avaliação e deve ser definido antes da execução do estudo de caso, experimento, prova de conceito, avaliação por especialistas ou teste com usuários.

#### 15.1.1 Objetivo do protocolo geral

O protocolo geral tem como objetivo padronizar a forma de validar propostas de naturezas diferentes, garantindo que toda avaliação contenha objeto, critérios, métricas, instrumentos, evidências, análise e limitações.

#### 15.1.2 Elementos mínimos do protocolo

| Elemento | Pergunta orientadora |

| --- | --- |

| Objeto de validação | O que exatamente será validado? |

| Tipo de proposta | É modelo, método, metodologia, arquitetura, framework, plataforma, pipeline, agente ou artefato? |

| Objetivo da validação | O que se pretende demonstrar? |

| Questões de avaliação | Quais perguntas a validação deve responder? |

| Critérios | Quais dimensões serão avaliadas? |

| Métricas | Como cada critério será medido? |

| Instrumentos | Quais checklists, questionários, logs, métricas, entrevistas ou testes serão usados? |

| Evidências | Que dados, registros, artefatos, logs ou opiniões serão coletados? |

| Participantes | Quem participa da validação? Especialistas, usuários, docentes, gestores, alunos ou desenvolvedores? |

| Procedimento | Quais etapas serão executadas? |

| Interpretação | Como os resultados serão analisados? |

| Limitações | Quais ameaças à validade serão registradas? |

#### 15.1.3 Delineamento geral da validação

Etapa 1 — Definir o objeto de validação

Deve-se explicitar se a proposta é um modelo, método, técnica, metodologia, arquitetura, framework, framework técnico-metodológico, plataforma, pipeline, agente inteligente ou artefato computacional.

Etapa 2 — Definir questões de avaliação

As questões de avaliação devem transformar a lacuna da pesquisa em perguntas verificáveis.

Exemplos:

A proposta é compreensível?

A proposta é aplicável?

A proposta melhora algo em relação a uma abordagem ad hoc?

A proposta produz os artefatos esperados?

A proposta é rastreável?

A proposta pode ser reproduzida?

A proposta é útil para especialistas ou usuários?

Etapa 3 — Definir critérios e métricas

Cada critério deve possuir métrica, indicador ou forma de avaliação.

Etapa 4 — Definir cenário de validação

O cenário pode ser real, simulado, experimental, prototípico ou baseado em especialistas.

Etapa 5 — Definir instrumentos

Podem ser usados checklists, matrizes, questionários, entrevistas, logs, testes, métricas computacionais, análise documental, prova de conceito ou estudo de caso.

Etapa 6 — Coletar evidências

As evidências devem ser quantitativas, qualitativas e documentais.

Etapa 7 — Interpretar resultados

Os resultados devem ser analisados com base nos critérios definidos.

Etapa 8 — Registrar limitações

Devem ser registradas ameaças à validade interna, externa, de construto e de conclusão.

#### 15.1.4 Matriz geral de validação

| Questão de avaliação | Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- | --- |

| A proposta atende aos requisitos? | Cobertura | requisitos atendidos / requisitos totais | matriz | tabela requisito-componente | mede completude |

| A proposta é aplicável? | Aplicabilidade | etapas executadas / etapas previstas | estudo de caso | relatório de aplicação | mede viabilidade |

| A proposta é útil? | Utilidade | nota média dos avaliadores | questionário | respostas | mede valor percebido |

| A proposta é rastreável? | Rastreabilidade | relações rastreáveis / relações esperadas | grafo/matriz | linhagem | mede auditabilidade |

| A proposta é reprodutível? | Reprodutibilidade | execuções reproduzidas / execuções testadas | reexecução | logs/resultados | mede repetibilidade |

### 15.2 Validação de modelo

Um modelo é uma representação abstrata de um fenômeno, estrutura, processo, dado, comportamento ou sistema. Pode ser conceitual, semântico, computacional, estatístico, preditivo, causal ou de referência. A validação de um modelo deve demonstrar que ele representa adequadamente aquilo que se propõe a representar.

#### 15.2.1 Objetivo da validação de modelo

A validação de modelo busca demonstrar que o modelo é claro, coerente, completo, aderente ao domínio, compreensível por especialistas e capaz de representar conceitos, relações, variáveis, processos ou fenômenos relevantes.

#### 15.2.2 Questões de avaliação

O modelo representa adequadamente os conceitos principais do domínio?

As relações entre os conceitos estão corretas?

Há conceitos ausentes, redundantes ou ambíguos?

O modelo é compreensível para especialistas e usuários?

O modelo pode ser aplicado em exemplos concretos?

O modelo está alinhado à literatura ou a modelos existentes?

O modelo ajuda a orientar análise, implementação ou decisão?

#### 15.2.3 Delineamento geral da validação

Etapa 1 — Definir o tipo de modelo

Deve-se indicar se o modelo é conceitual, semântico, computacional, estatístico, preditivo, causal ou de referência.

Exemplos:

No UnespDataLens, pode-se validar um modelo conceitual de organização de conceitos.

No SemED-LLM, pode-se validar um modelo semântico de lacunas conceituais.

Na MILA-eDU, pode-se validar um modelo analítico de apoio à decisão.

No FairED-Pipeline, pode-se validar um modelo de categorias de vieses.

No GeoReXAI, pode-se validar um modelo geoespacial explicável.

Etapa 2 — Definir conceitos, entidades ou variáveis

O modelo deve listar seus elementos centrais e suas definições.

Etapa 3 — Definir relações

As relações entre os elementos devem ser explicitadas, justificadas e exemplificadas.

Etapa 4 — Construir matriz conceitual

| Conceito | Definição | Relações | Justificativa | Exemplo | Status |

| --- | --- | --- | --- | --- | --- |

Etapa 5 — Comparar com literatura ou taxonomias existentes

O pesquisador deve verificar se o modelo está alinhado ao estado da arte.

Etapa 6 — Aplicar o modelo em exemplos

O modelo deve ser testado em exemplos reais, simulados ou prototípicos.

Etapa 7 — Avaliar por especialistas

Especialistas devem avaliar clareza, completude, coerência, aderência e utilidade.

Etapa 8 — Revisar o modelo

Conceitos ausentes, ambíguos ou redundantes devem ser revisados.

#### 15.2.4 Métricas para validação de modelo

Clareza conceitual

Clareza Conceitual = soma das notas atribuídas / pontuação máxima possível

Completude conceitual

Completude Conceitual = conceitos contemplados / conceitos esperados

Coerência relacional

Coerência Relacional = relações aceitas / relações avaliadas

Ambiguidade conceitual

Ambiguidade = conceitos ambíguos / conceitos totais

Quanto menor a ambiguidade, melhor.

Aplicabilidade do modelo

Aplicabilidade = casos representados corretamente / casos avaliados

#### 15.2.5 Matriz rigorosa de avaliação de modelo

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Clareza | nota média dos avaliadores | questionário | respostas | mede compreensibilidade |

| Completude | conceitos contemplados / esperados | checklist | matriz conceitual | mede cobertura |

| Coerência | relações aceitas / avaliadas | parecer especializado | análise das relações | mede consistência |

| Ambiguidade | conceitos ambíguos / totais | análise documental | glossário | mede precisão conceitual |

| Aplicabilidade | casos representados / avaliados | estudo de aplicação | exemplos resolvidos | mede uso prático |

| Utilidade | nota média dos usuários | questionário | feedback | mede valor percebido |

#### 15.2.6 Delineamento por tipo de modelo

Modelo conceitual

| Dimensão | Métrica |

| --- | --- |

| Clareza | nota média dos avaliadores |

| Completude | conceitos contemplados / esperados |

| Coerência | relações aceitas / avaliadas |

| Ambiguidade | conceitos ambíguos / totais |

Modelo semântico

| Dimensão | Métrica |

| --- | --- |

| Cobertura semântica | categorias representadas / necessárias |

| Coerência semântica | relações semânticas aceitas / avaliadas |

| Precisão terminológica | termos adequados / termos avaliados |

| Utilidade pedagógica | nota média de usuários |

Modelo preditivo ou estatístico

| Dimensão | Métrica |

| --- | --- |

| Classificação | acurácia, precisão, recall, F1, AUC |

| Regressão | MAE, RMSE, R² |

| Estabilidade | variação das métricas entre execuções |

| Fairness | SPD, DI, EOD, AOD, FPR/FNR por grupo |

Modelo causal ou decisório

| Dimensão | Métrica |

| --- | --- |

| Clareza das relações | relações validadas / relações propostas |

| Plausibilidade causal | relações plausíveis / relações avaliadas |

| Utilidade decisória | nota média dos gestores |

| Rastreabilidade | decisões com evidência / decisões totais |

#### 15.2.7 Exemplos de aplicação

No UnespDataLens, um modelo conceitual pode ser validado solicitando que alunos localizem conceitos e expliquem relações entre método, técnica, metodologia, arquitetura e framework.

No SemED-LLM, um modelo semântico pode ser validado comparando categorias de lacunas conceituais com classificações feitas por docentes.

Na MILA-eDU, um modelo decisório pode ser validado verificando se gestores conseguem relacionar fatores de evasão, indicadores e possíveis ações.

No FairED-Pipeline, um modelo de vieses pode ser validado verificando se especialistas reconhecem as categorias de viés propostas.

#### 15.2.8 Relatório de validação de modelo

O relatório deve conter:

tipo de modelo validado;

conceitos e relações avaliadas;

critérios e métricas;

instrumentos utilizados;

especialistas ou usuários participantes;

resultados quantitativos;

comentários qualitativos;

conceitos revisados;

limitações;

versão final do modelo.

#### 15.2.9 Síntese

Um modelo bem validado não é apenas visualmente compreensível. Ele deve demonstrar, por meio de métricas, pareceres, exemplos e matriz conceitual, que representa adequadamente o fenômeno ou estrutura que pretende descrever.

### 15.3 Validação de modelo de referência

Um modelo de referência é uma estrutura abstrata, reutilizável e generalizável que orienta diferentes instanciações de uma classe de soluções. Sua validação deve demonstrar que o modelo é completo, coerente, aplicável, adaptável e capaz de orientar arquiteturas, frameworks, plataformas ou pipelines.

#### 15.3.1 Objetivo da validação de modelo de referência

A validação de modelo de referência busca demonstrar que seus princípios, componentes, artefatos, metadados, contratos, relações, critérios e dimensões transversais são suficientes para orientar uma classe de soluções.

#### 15.3.2 Questões de avaliação

O modelo contempla os elementos essenciais da classe de problemas?

Os princípios, componentes, artefatos, metadados e contratos estão claros?

O modelo pode ser instanciado em diferentes cenários?

Há elementos redundantes ou ausentes?

O modelo está alinhado com literatura, padrões ou boas práticas?

O modelo permite adaptação sem perder coerência?

O modelo facilita implementação, documentação e avaliação?

#### 15.3.3 Delineamento geral da validação

Etapa 1 — Definir os elementos formais

O modelo deve explicitar:

princípios;

componentes;

artefatos;

metadados;

contratos;

relações;

critérios de avaliação;

dimensões transversais.

Etapa 2 — Construir matriz lacuna–elemento

| Lacuna/Requisito | Elemento do modelo | Justificativa | Evidência esperada |

| --- | --- | --- | --- |

Etapa 3 — Comparar com estruturas relacionadas

Comparar com frameworks, arquiteturas, padrões ou metodologias existentes.

Etapa 4 — Instanciar o modelo

Aplicar o modelo em pelo menos um cenário real, simulado ou prototípico.

Etapa 5 — Avaliar suficiência dos elementos

Verificar se os elementos previstos foram suficientes para orientar a instanciação.

Etapa 6 — Avaliar por especialistas

Especialistas avaliam clareza, completude, aplicabilidade, generalidade e utilidade.

Etapa 7 — Revisar o modelo

Registrar inclusão, remoção, fusão ou redefinição de elementos.

#### 15.3.4 Métricas para validação de modelo de referência

Cobertura de lacunas

Cobertura de Lacunas = lacunas atendidas / lacunas identificadas

Cobertura de elementos

Cobertura de Elementos = elementos instanciados / elementos previstos

Índice de redundância

Redundância = elementos sobrepostos / elementos totais

Generalidade

Generalidade = cenários compatíveis / cenários avaliados

Aplicabilidade

Aplicabilidade = elementos utilizados / elementos aplicáveis

#### 15.3.5 Matriz rigorosa de avaliação de modelo de referência

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Cobertura | lacunas atendidas / total | matriz lacuna-elemento | tabela de mapeamento | mede alinhamento ao problema |

| Completude | elementos previstos / necessários | checklist | modelo formal | mede suficiência |

| Aplicabilidade | elementos utilizados / aplicáveis | estudo de caso | relatório de instanciação | mede viabilidade |

| Generalidade | cenários compatíveis / avaliados | múltiplos cenários | relatório comparativo | mede adaptação |

| Redundância | elementos sobrepostos / total | análise conceitual | relatório de revisão | mede excesso estrutural |

| Clareza | nota média | especialistas | questionário | mede compreensibilidade |

#### 15.3.6 Delineamento por tipo de modelo de referência

Modelo de referência para pipelines

| Dimensão | Métrica |

| --- | --- |

| Cobertura de etapas | etapas contempladas / etapas necessárias |

| Artefatos | artefatos definidos / artefatos esperados |

| Metadados | tipos de metadados contemplados / necessários |

| Rastreabilidade | relações previstas / relações esperadas |

Modelo de referência para apoio à decisão

| Dimensão | Métrica |

| --- | --- |

| Cobertura decisória | decisões apoiadas / decisões previstas |

| Evidências | recomendações com evidência / recomendações totais |

| Interpretabilidade | nota média dos gestores |

| Aplicabilidade | etapas utilizadas / etapas aplicáveis |

Modelo de referência para plataforma de conhecimento

| Dimensão | Métrica |

| --- | --- |

| Cobertura conceitual | conceitos representados / conceitos previstos |

| Navegação semântica | links corretos / links avaliados |

| Reuso | itens reutilizáveis / itens totais |

| Utilidade | nota média dos usuários |

#### 15.3.7 Exemplos de aplicação

No EdmLens, o modelo de referência pode ser validado verificando se seus elementos orientam a construção de pipelines educacionais rastreáveis, governados e catalogáveis.

Na MILA-eDU, o modelo de referência pode ser validado verificando se orienta a passagem entre problema educacional, indicadores, análise, decisão, ação e avaliação.

No UnespDataLens, o modelo de referência pode ser validado verificando se orienta a organização de conceitos, métodos, técnicas, exemplos, links e módulos de aprendizagem.

#### 15.3.8 Relatório de validação de modelo de referência

O relatório deve conter:

elementos do modelo de referência;

lacunas associadas;

matriz lacuna–elemento;

cenários de instanciação;

métricas calculadas;

avaliação por especialistas;

elementos revisados;

limitações de generalização.

#### 15.3.9 Síntese

Um modelo de referência validado deve demonstrar que seus elementos são suficientes para orientar uma classe de soluções, e não apenas uma aplicação isolada.

### 15.4 Validação de método

Um método é um procedimento sistemático para realizar uma tarefa específica. Diferentemente de uma metodologia, que organiza um processo amplo, o método possui objetivo operacional delimitado.

#### 15.4.1 Objetivo da validação de método

A validação de método busca demonstrar que o procedimento proposto executa corretamente uma tarefa específica, com desempenho, robustez, eficiência, estabilidade e adequação ao domínio.

#### 15.4.2 Questões de avaliação

O método executa a tarefa para a qual foi proposto?

O método melhora resultados em relação a uma alternativa?

O método é robusto a diferentes cenários ou dados?

O método apresenta custo computacional adequado?

O método produz saídas interpretáveis ou úteis?

O método possui limitações claras?

O método pode ser reproduzido?

#### 15.4.3 Delineamento geral da validação

Etapa 1 — Definir a tarefa do método

Exemplos:

detectar drift;

classificar lacunas conceituais;

mitigar viés;

explicar uma predição;

integrar dados;

calcular indicador;

ranquear alternativas.

Etapa 2 — Definir entradas e saídas

O método deve possuir entradas, saídas e condições de aplicação.

Etapa 3 — Definir baseline

Sempre que possível, comparar com método existente, abordagem simples ou execução manual.

Etapa 4 — Preparar dados ou cenários

Os dados podem ser reais, simulados, sintéticos ou de benchmark.

Etapa 5 — Aplicar o método

Executar o método e registrar parâmetros, versões e ambiente.

Etapa 6 — Medir desempenho

Aplicar métricas adequadas à tarefa.

Etapa 7 — Analisar erros

Identificar casos de sucesso, falha e condições de limitação.

Etapa 8 — Comparar com baseline

Avaliar ganho, perda ou trade-off.

#### 15.4.4 Métricas para validação de método

Efetividade

Efetividade = casos corretos / casos avaliados

Pode ser substituída por F1, acurácia, recall, precisão, RMSE ou outra métrica específica.

Ganho em relação ao baseline

Ganho Relativo = (métrica_proposta - métrica_baseline) / métrica_baseline

Eficiência

Eficiência = tempo de execução ou uso de recursos computacionais

Robustez

Robustez = desempenho médio em diferentes cenários

Também pode ser avaliada pelo desvio padrão entre cenários.

Sensibilidade

Sensibilidade = variação da saída em função da variação de parâmetros

#### 15.4.5 Matriz rigorosa de avaliação de método

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Efetividade | F1, acurácia ou redução de erro | experimento | resultados | mede se o método funciona |

| Eficiência | tempo/memória | monitoramento | logs | mede custo |

| Robustez | variação entre cenários | testes múltiplos | tabela comparativa | mede estabilidade contextual |

| Sensibilidade | variação por parâmetro | análise experimental | gráficos/tabelas | mede dependência de configuração |

| Comparabilidade | ganho relativo | baseline | tabela comparativa | mede avanço |

| Utilidade | nota média | especialista/usuário | questionário | mede valor prático |

#### 15.4.6 Delineamento por tipo de método

Método de classificação

| Dimensão | Métrica |

| --- | --- |

| Desempenho | acurácia, precisão, recall, F1 |

| Erro | matriz de confusão |

| Robustez | variação entre folds |

| Comparação | ganho sobre baseline |

Método de explicabilidade

| Dimensão | Métrica |

| --- | --- |

| Estabilidade | variação das explicações |

| Fidelidade | aderência ao modelo explicado |

| Utilidade | nota de especialistas |

| Clareza | nota de interpretabilidade |

Método de mitigação de vieses

| Dimensão | Métrica |

| --- | --- |

| Fairness | SPD, DI, EOD, AOD |

| Desempenho | F1, AUC, recall |

| Trade-off | perda de desempenho versus ganho de fairness |

| Estabilidade | variação entre grupos |

#### 15.4.7 Exemplos de aplicação

Um método de detecção de drift no EdmLens pode ser validado criando cenários com mudança conhecida na distribuição dos dados.

Um método de mitigação de vieses no FairED-Pipeline pode ser validado comparando métricas de fairness antes e depois da mitigação.

Um método de classificação semântica no SemED-LLM pode ser validado comparando a saída do método com classificações docentes.

#### 15.4.8 Relatório de validação de método

O relatório deve conter:

tarefa do método;

dados ou cenários usados;

baseline;

parâmetros;

métricas;

resultados;

análise de erro;

comparação;

limitações;

recomendação de uso.

#### 15.4.9 Síntese

Um método validado deve demonstrar que executa uma tarefa específica de forma mensurável, comparável e reprodutível.

### 15.5 Validação de metodologia

Uma metodologia organiza etapas, atividades, papéis, critérios e produtos para conduzir um processo. Sua validação deve verificar se ela orienta adequadamente a execução de uma atividade complexa.

#### 15.5.1 Objetivo da validação de metodologia

A validação de metodologia busca demonstrar que suas etapas são claras, aplicáveis, completas, úteis, reproduzíveis e capazes de conduzir o usuário de um problema inicial até um resultado documentado e avaliável.

#### 15.5.2 Questões de avaliação

As etapas da metodologia são claras?

Cada etapa possui entrada, atividade, saída e responsável?

A metodologia pode ser aplicada em um caso real ou simulado?

As saídas esperadas são produzidas?

A metodologia ajuda a organizar decisões?

Os usuários conseguem seguir o processo?

A metodologia é flexível o suficiente para adaptação?

O processo pode ser documentado e reproduzido?

#### 15.5.3 Delineamento geral da validação

Etapa 1 — Descrever formalmente as etapas

Cada etapa deve ter objetivo, entrada, atividade, saída e responsável.

| Etapa | Entrada | Atividade | Saída | Responsável |

| --- | --- | --- | --- | --- |

Etapa 2 — Definir critérios de sucesso por etapa

Exemplo: etapa concluída, artefato produzido, decisão registrada, validação realizada.

Etapa 3 — Aplicar a metodologia em um caso

O caso pode ser real, simulado ou prototípico.

Etapa 4 — Registrar execução

Documentar quais etapas foram executadas, quais foram adaptadas e quais dificuldades ocorreram.

Etapa 5 — Coletar artefatos

Cada etapa deve produzir evidências.

Etapa 6 — Coletar feedback

Participantes avaliam clareza, utilidade, esforço e aplicabilidade.

Etapa 7 — Revisar a metodologia

As etapas devem ser ajustadas com base nos resultados.

#### 15.5.4 Métricas para validação de metodologia

Aderência às etapas

Aderência = etapas executadas / etapas previstas

Completude das saídas

Completude das Saídas = saídas produzidas / saídas esperadas

Clareza metodológica

Clareza = soma das notas dos avaliadores / pontuação máxima possível

Esforço de aplicação

Esforço = tempo total de aplicação ou tempo por etapa

Capacidade de orientação

Capacidade de Orientação = decisões apoiadas / decisões previstas

#### 15.5.5 Matriz rigorosa de avaliação de metodologia

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Aderência | etapas executadas / previstas | checklist | registro de aplicação | mede execução |

| Completude | saídas produzidas / esperadas | matriz etapa-saída | artefatos | mede produtividade |

| Clareza | nota média | questionário | respostas | mede compreensão |

| Utilidade | nota média | usuários/especialistas | feedback | mede valor percebido |

| Reprodutibilidade | etapas documentadas / executadas | análise documental | relatório | mede repetição |

| Flexibilidade | adaptações bem-sucedidas / necessárias | relatório | registro de ajustes | mede adaptabilidade |

#### 15.5.6 Delineamento por tipo de metodologia

Metodologia analítica de apoio à decisão

Aplicável à MILA-eDU.

| Dimensão | Métrica |

| --- | --- |

| Aderência | etapas executadas / previstas |

| Evidência decisória | decisões com evidência / decisões totais |

| Utilidade | nota média dos gestores |

| Rastreabilidade | recomendações rastreáveis / recomendações totais |

Metodologia de avaliação de vieses

Aplicável ao FairED-Pipeline.

| Dimensão | Métrica |

| --- | --- |

| Cobertura de etapas | etapas executadas / previstas |

| Métricas aplicadas | métricas calculadas / métricas previstas |

| Mitigação | disparidades reduzidas / disparidades identificadas |

| Documentação | registros produzidos / registros esperados |

Metodologia de diagnóstico semântico

Aplicável ao SemED-LLM.

| Dimensão | Métrica |

| --- | --- |

| Taxonomia | categorias validadas / categorias propostas |

| Validação humana | respostas validadas / respostas avaliadas |

| Concordância | classificações concordantes / total |

| Utilidade pedagógica | nota média dos docentes |

#### 15.5.7 Exemplos de aplicação

A MILA-eDU pode ser validada aplicando suas etapas a um problema de evasão, verificando se a metodologia conduz da identificação do problema até a priorização de ações.

Uma metodologia para fairness pode ser validada aplicando suas etapas em diferentes datasets educacionais.

Uma metodologia para diagnóstico semântico com LLMs pode ser validada verificando se docentes conseguem aplicar o processo de taxonomia, prompt, classificação e validação.

#### 15.5.8 Relatório de validação de metodologia

O relatório deve conter:

etapas da metodologia;

caso de aplicação;

participantes;

artefatos por etapa;

métricas;

dificuldades;

adaptações;

feedback;

versão revisada.

#### 15.5.9 Síntese

Uma metodologia bem validada deve demonstrar que orienta a execução de um processo, produz artefatos úteis e pode ser aplicada por outros usuários além do autor da proposta.

### 15.6 Validação de arquitetura

Uma arquitetura deve ser validada quanto à sua capacidade de organizar adequadamente uma solução computacional. O objetivo da validação arquitetural é verificar se os componentes propostos são necessários, suficientes, coerentes, bem relacionados, implementáveis e capazes de atender aos requisitos funcionais, técnicos, metodológicos e de governança da proposta.

#### 15.6.1 Objetivo da validação arquitetural

A validação arquitetural busca responder se a arquitetura contempla os requisitos relevantes da proposta, se os módulos são necessários e suficientes, se as responsabilidades estão bem distribuídas, se os fluxos são coerentes, se há governança e rastreabilidade quando necessárias, e se a arquitetura pode ser implementada, compreendida, mantida e evoluída.

#### 15.6.2 Questões de avaliação

A arquitetura contempla todos os requisitos relevantes?

Os componentes ou módulos são necessários e suficientes?

As responsabilidades estão bem distribuídas?

Há sobreposição indevida entre componentes?

As dependências entre módulos estão claras?

Os fluxos de dados, processos, artefatos ou decisões estão coerentes?

A arquitetura permite implementação?

A arquitetura permite evolução, extensão e manutenção?

A arquitetura contempla governança, segurança, rastreabilidade e reprodutibilidade?

A arquitetura é compreensível para os stakeholders?

#### 15.6.3 Delineamento geral da validação

Etapa 1 — Definir o escopo arquitetural

Delimitar se será validada a arquitetura completa, um subconjunto de módulos, uma visão específica, um fluxo de dados, uma arquitetura de agentes, de plataforma, de pipeline ou de apoio à decisão.

Etapa 2 — Definir requisitos arquiteturais

| Código | Requisito | Tipo |

| --- | --- | --- |

| RQ-A01 | A arquitetura deve permitir entrada de múltiplas fontes de dados | Funcional |

| RQ-A02 | A arquitetura deve registrar metadados dos artefatos | Técnico |

| RQ-A03 | A arquitetura deve permitir rastreabilidade entre entrada e saída | Proveniência |

| RQ-A04 | A arquitetura deve prever controle de acesso | Governança |

| RQ-A05 | A arquitetura deve permitir expansão de módulos | Evolução |

| RQ-A06 | A arquitetura deve ser compreensível para usuários técnicos e especialistas | Usabilidade arquitetural |

Etapa 3 — Construir matriz requisito-componente

Cada requisito deve ser mapeado para um ou mais componentes.

| Requisito | Componente responsável | Evidência | Status |

| --- | --- | --- | --- |

Etapa 4 — Avaliar múltiplas visões arquiteturais

| Visão | O que avaliar | Evidência |

| --- | --- | --- |

| Conceitual | Conceitos e relações do domínio | Diagrama conceitual, glossário |

| Lógica | Módulos e responsabilidades | Diagrama de módulos |

| Dados | Entidades, schemas, metadados | Modelo de dados, dicionário |

| Processo | Fluxo de execução | Diagrama de pipeline/workflow |

| Implementação | Tecnologias e estrutura de código | Repositório, protótipo |

| Governança | Papéis, políticas e restrições | Matriz de acesso, regras |

| Proveniência | Linhagem e dependências | Grafo de linhagem |

| Monitoramento | Estados, alertas e evolução | Plano de monitoramento |

Etapa 5 — Aplicar métricas arquiteturais

A avaliação deve usar métricas quantitativas, qualitativas ou semiquantitativas.

Etapa 6 — Realizar inspeção técnica

Especialistas, orientadores, desenvolvedores ou pares devem avaliar a arquitetura por formulário estruturado.

Etapa 7 — Executar cenários de validação

Exemplos:

um novo dataset é inserido;

uma feature apresenta drift;

um prompt gera resposta fora da taxonomia;

um usuário busca um conceito;

uma métrica de fairness indica disparidade.

Etapa 8 — Construir prova de conceito

Sempre que possível, implementar versão mínima para verificar viabilidade.

Etapa 9 — Revisar a arquitetura

A validação deve gerar mudanças justificadas: inclusão, exclusão, fusão, separação ou redefinição de componentes.

#### 15.6.4 Métricas para validação de arquitetura

Cobertura de requisitos

Cobertura de Requisitos = requisitos atendidos / requisitos totais

Cobertura de componentes

Cobertura de Componentes = componentes associados a requisitos / componentes totais

Índice de lacunas

Índice de Lacunas = requisitos não atendidos / requisitos totais

Redundância

Redundância = responsabilidades duplicadas / responsabilidades totais

Acoplamento médio

Acoplamento Médio = dependências totais / componentes totais

Cobertura de rastreabilidade

Cobertura de Rastreabilidade = relações rastreáveis / relações esperadas

#### 15.6.5 Matriz rigorosa de avaliação arquitetural

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Cobertura de requisitos | requisitos atendidos / total | matriz requisito-componente | tabela de mapeamento | mede completude |

| Cobertura de componentes | componentes justificados / total | matriz componente-requisito | lista de módulos | identifica módulos sem função |

| Lacunas | requisitos não atendidos / total | checklist | relatório de lacunas | mede ausência arquitetural |

| Redundância | responsabilidades duplicadas / total | matriz de responsabilidades | análise de sobreposição | mede duplicação |

| Coesão | nota média por componente | avaliação técnica | rubrica de coesão | mede foco interno |

| Acoplamento | dependências / componentes | grafo de dependência | diagrama ou matriz | mede dependência |

| Clareza | pontuação média | questionário | avaliação de especialistas | mede compreensibilidade |

| Governança | itens atendidos / necessários | checklist de governança | política e logs | mede controle |

| Rastreabilidade | relações rastreáveis / esperadas | grafo de linhagem | trilha fonte–saída | mede auditabilidade |

| Implementabilidade | escala 1–5 | revisão técnica | prova de conceito | mede viabilidade |

| Extensibilidade | cenários suportados / propostos | cenários de evolução | relatório de adaptação | mede capacidade de evolução |

#### 15.6.6 Delineamento por tipo de arquitetura

Arquitetura de pipeline de dados

Aplicável a EdmLens, EduPipeX e FairED-Pipeline.

| Dimensão | Métrica |

| --- | --- |

| Fluxo | etapas executáveis / etapas previstas |

| Qualidade | datasets com relatório de qualidade / datasets gerados |

| Rastreabilidade | artefatos com linhagem / artefatos totais |

| Metadados | campos preenchidos / campos obrigatórios |

| Contratos | contratos satisfeitos / contratos definidos |

| Reprodutibilidade | execuções reproduzidas / execuções testadas |

Arquitetura de plataforma

Aplicável a UnespDataLens, plataforma MILA-eDU ou plataforma EdmLens.

| Dimensão | Métrica |

| --- | --- |

| Funcionalidade | funcionalidades implementadas / funcionalidades previstas |

| Efetividade | tarefas concluídas com sucesso / tarefas totais |

| Eficiência | tempo médio para completar tarefa |

| Navegabilidade | cliques até encontrar informação |

| Erros | erros por tarefa |

| Satisfação | nota média dos usuários |

| Cobertura de conteúdo | itens documentados / itens previstos |

Arquitetura com LLMs ou agentes

Aplicável ao SemED-LLM e agentes do UnespDataLens, EdmLens ou FairED-Pipeline.

| Dimensão | Métrica |

| --- | --- |

| Rastreabilidade | respostas com prompt registrado / respostas totais |

| Validação humana | respostas validadas / respostas amostradas |

| Conformidade | respostas no formato esperado / respostas totais |

| Desempenho | F1, acurácia, precisão, recall |

| Consistência | respostas equivalentes em execuções repetidas |

| Segurança | violações de restrição / total de execuções |

| Alucinação | respostas incorretas / respostas avaliadas |

| Autonomia | ações dentro do nível permitido / ações totais |

Arquitetura geoespacial explicável

Aplicável ao GeoReXAI.

| Dimensão | Métrica |

| --- | --- |

| Validade espacial | geometrias válidas / geometrias totais |

| Cobertura espacial | área coberta / área esperada |

| Qualidade preditiva | RMSE, MAE, R² |

| Explicabilidade | mapas úteis / mapas avaliados |

| Rastreabilidade | mapas com linhagem completa / mapas totais |

| Consistência espacial | avaliação por especialista |

| Clareza visual | nota média dos usuários |

Arquitetura de apoio à decisão

Aplicável à MILA-eDU.

| Dimensão | Métrica |

| --- | --- |

| Cobertura decisória | decisões apoiadas / decisões previstas |

| Rastreabilidade | recomendações com evidência associada / recomendações totais |

| Utilidade | nota média dos gestores |

| Clareza | usuários que compreendem o fluxo / usuários totais |

| Tempo de análise | tempo para chegar a uma recomendação |

| Qualidade da recomendação | avaliação por especialistas |

| Aderência metodológica | etapas executadas / etapas previstas |

#### 15.6.7 Exemplos de aplicação

No EdmLens, pode-se validar a arquitetura por meio de um pipeline educacional de evasão, verificando cobertura de módulos, metadados, contratos, linhagem, governança e reprodutibilidade.

No SemED-LLM, pode-se validar se a arquitetura rastreia texto, prompt, modelo, resposta, validação docente e explicação.

No UnespDataLens, pode-se validar se usuários conseguem localizar conceitos, acessar exemplos, navegar entre módulos e compreender relações semânticas.

#### 15.6.8 Relatório de validação arquitetural

O relatório deve conter:

descrição da arquitetura;

requisitos arquiteturais;

stakeholders e preocupações;

visões avaliadas;

matriz requisito-componente;

métricas calculadas;

lacunas identificadas;

redundâncias;

trade-offs;

alterações realizadas.

#### 15.6.9 Síntese

Uma arquitetura validada deve demonstrar, com métricas, matrizes e cenários, que seus componentes são necessários, suficientes, coerentes e implementáveis.

### 15.7 Validação de framework

Um framework é uma estrutura organizada e reutilizável para tratar uma classe de problemas. Sua validação deve demonstrar que ele é compreensível, aplicável, completo, reutilizável, adaptável e capaz de orientar a produção de artefatos coerentes.

#### 15.7.1 Objetivo da validação de framework

A validação de framework busca demonstrar que a estrutura proposta orienta adequadamente uma classe de problemas, e não apenas um caso isolado.

#### 15.7.2 Questões de avaliação

O framework define claramente a classe de problemas?

Seus princípios, módulos, processos e artefatos estão claros?

O framework pode ser instanciado em um cenário?

Os módulos são suficientes para orientar a solução?

A aplicação do framework produz artefatos úteis?

O framework é reutilizável ou adaptável?

O framework melhora a organização em relação a uma abordagem ad hoc?

Especialistas compreendem e consideram o framework útil?

#### 15.7.3 Delineamento geral da validação

Etapa 1 — Definir a classe de problemas

Exemplos:

engenharia de dados educacionais;

diagnóstico semântico;

fairness em pipelines;

explicabilidade geoespacial;

apoio à decisão;

explicabilidade de pipelines.

Etapa 2 — Formalizar princípios, módulos e artefatos

O framework deve explicitar sua estrutura.

Etapa 3 — Definir critérios de aderência

Criar checklist para avaliar se uma instanciação segue o framework.

Etapa 4 — Instanciar o framework

Aplicar em cenário real, simulado ou prototípico.

Etapa 5 — Avaliar artefatos produzidos

Verificar qualidade, utilidade, completude, documentação e rastreabilidade.

Etapa 6 — Comparar com abordagem alternativa

Quando possível, comparar com abordagem ad hoc ou framework existente.

Etapa 7 — Avaliar por especialistas

Coletar avaliação estruturada.

Etapa 8 — Revisar o framework

Ajustar módulos, artefatos, processos ou critérios.

#### 15.7.4 Métricas para validação de framework

Aderência ao framework

Aderência = módulos aplicados / módulos previstos

Completude estrutural

Completude = elementos especificados / elementos esperados

Aplicabilidade

Aplicabilidade = etapas executadas / etapas planejadas

Reutilização

Reutilização = artefatos reutilizáveis / artefatos gerados

Rastreabilidade

Rastreabilidade = relações rastreáveis / relações esperadas

#### 15.7.5 Matriz rigorosa de avaliação de framework

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Aderência | módulos aplicados / previstos | checklist | relatório de aplicação | mede uso do framework |

| Completude | elementos especificados / esperados | matriz | documentação | mede suficiência |

| Aplicabilidade | etapas executadas / planejadas | estudo de caso | artefatos | mede viabilidade |

| Reuso | artefatos reutilizáveis / gerados | análise documental | repositório | mede reutilização |

| Utilidade | nota média | especialistas/usuários | questionário | mede valor percebido |

| Rastreabilidade | relações rastreáveis / esperadas | grafo/matriz | linhagem | mede auditabilidade |

#### 15.7.6 Delineamento por tipo de framework

Framework de engenharia de dados

Aplicável ao EdmLens.

| Dimensão | Métrica |

| --- | --- |

| Módulos | módulos aplicados / previstos |

| Metadados | campos preenchidos / obrigatórios |

| Governança | políticas aplicadas / necessárias |

| Proveniência | relações rastreáveis / esperadas |

Framework de diagnóstico semântico

Aplicável ao SemED-LLM.

| Dimensão | Métrica |

| --- | --- |

| Taxonomia | categorias aplicadas / categorias previstas |

| Prompts | prompts versionados / prompts utilizados |

| Validação humana | respostas validadas / amostra |

| Utilidade docente | nota média dos docentes |

Framework de fairness

Aplicável ao FairED-Pipeline.

| Dimensão | Métrica |

| --- | --- |

| Métricas | métricas calculadas / métricas previstas |

| Grupos | grupos analisados / grupos relevantes |

| Mitigação | disparidades reduzidas / disparidades identificadas |

| Auditoria | registros produzidos / registros esperados |

#### 15.7.7 Exemplos de aplicação

O EdmLens pode ser validado por instanciação em um pipeline de evasão, desempenho ou engajamento.

O SemED-LLM pode ser validado com interações textuais reais ou simuladas.

O FairED-Pipeline pode ser validado em diferentes datasets educacionais.

#### 15.7.8 Relatório de validação de framework

O relatório deve conter:

classe de problemas;

módulos do framework;

cenário de instanciação;

checklist de aderência;

artefatos produzidos;

métricas calculadas;

avaliação por especialistas;

comparação com baseline;

limitações;

ajustes realizados.

#### 15.7.9 Síntese

Um framework validado deve demonstrar que orienta uma classe de problemas, produz artefatos úteis e pode ser reutilizado ou adaptado.

### 15.8 Validação de framework técnico-metodológico

Um framework técnico-metodológico combina estrutura técnica e orientação metodológica. Sua validação deve avaliar simultaneamente arquitetura, modelo de referência, módulos, artefatos, metadados, contratos, governança, rastreabilidade, reprodutibilidade e diretrizes de aplicação.

#### 15.8.1 Objetivo da validação de framework técnico-metodológico

Demonstrar que o framework não apenas organiza componentes técnicos, mas também orienta sua aplicação, documentação, implementação, avaliação, governança e evolução.

#### 15.8.2 Questões de avaliação

O framework possui definição conceitual clara?

O modelo de referência é completo?

A arquitetura modular é coerente?

Os módulos estão suficientemente especificados?

Os artefatos, metadados e contratos estão definidos?

O framework orienta implementação ou instanciação?

O framework registra governança, proveniência e rastreabilidade?

O framework favorece reprodutibilidade?

O framework é útil para especialistas ou usuários?

Pode ser adaptado a outros cenários?

#### 15.8.3 Delineamento geral da validação

Etapa 1 — Validar definição conceitual

Verificar se a proposta está corretamente caracterizada como framework técnico-metodológico.

Etapa 2 — Validar modelo de referência

Avaliar princípios, módulos, artefatos, metadados, contratos, relações e critérios.

Etapa 3 — Validar arquitetura

Aplicar métricas arquiteturais.

Etapa 4 — Validar especificação dos módulos

Verificar entradas, saídas, responsabilidades, contratos, erros e métricas.

Etapa 5 — Instanciar o framework

Aplicar em cenário real ou prototípico.

Etapa 6 — Avaliar artefatos e metadados

Medir completude, qualidade e rastreabilidade.

Etapa 7 — Avaliar utilidade

Coletar percepção de especialistas e usuários.

Etapa 8 — Avaliar reprodutibilidade

Reexecutar ou simular reexecução.

Etapa 9 — Revisar o framework

Registrar melhorias e limitações.

#### 15.8.4 Métricas para validação de framework técnico-metodológico

Cobertura do modelo de referência

Cobertura do Modelo = elementos instanciados / elementos previstos

Cobertura modular

Cobertura Modular = módulos especificados / módulos previstos

Completude da especificação

Completude da Especificação = campos preenchidos / campos obrigatórios

Cobertura de metadados

Cobertura de Metadados = metadados preenchidos / metadados obrigatórios

Satisfação de contratos

Satisfação de Contratos = contratos atendidos / contratos testados

Reprodutibilidade

Reprodutibilidade = execuções reproduzidas / execuções testadas

#### 15.8.5 Matriz rigorosa de avaliação de framework técnico-metodológico

| Dimensão | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Modelo de referência | elementos instanciados / previstos | matriz | relatório | mede aplicabilidade conceitual |

| Arquitetura | requisitos atendidos / total | matriz requisito-módulo | diagrama | mede completude |

| Módulos | módulos especificados / previstos | checklist | documentação | mede formalização |

| Metadados | campos preenchidos / obrigatórios | análise documental | registros | mede documentação |

| Contratos | contratos atendidos / testados | execução | logs | mede implementabilidade |

| Rastreabilidade | relações rastreáveis / esperadas | grafo | linhagem | mede auditabilidade |

| Reprodutibilidade | execuções reproduzidas / testadas | reexecução | resultados | mede repetibilidade |

| Utilidade | nota média | especialistas | questionário | mede valor percebido |

#### 15.8.6 Delineamento por tipo de framework técnico-metodológico

Framework técnico-metodológico de dados educacionais

Aplicável ao EdmLens.

| Dimensão | Métrica |

| --- | --- |

| Módulos | módulos especificados / módulos previstos |

| Artefatos | artefatos gerados / artefatos esperados |

| Metadados | metadados preenchidos / obrigatórios |

| Proveniência | relações rastreáveis / esperadas |

| Governança | políticas aplicadas / necessárias |

Framework técnico-metodológico de fairness

Aplicável ao FairED-Pipeline.

| Dimensão | Métrica |

| --- | --- |

| Etapas | etapas executadas / etapas previstas |

| Métricas | métricas de fairness calculadas / previstas |

| Mitigação | disparidades reduzidas / identificadas |

| Documentação | registros produzidos / esperados |

| Monitoramento | alertas identificados / esperados |

Framework técnico-metodológico com LLMs

Aplicável ao SemED-LLM.

| Dimensão | Métrica |

| --- | --- |

| Prompts | prompts versionados / utilizados |

| Respostas | respostas rastreáveis / respostas totais |

| Validação humana | respostas validadas / amostra |

| Segurança | violações / execuções |

| Utilidade pedagógica | nota média dos docentes |

#### 15.8.7 Exemplos de aplicação

O EdmLens pode ser validado por instanciação em pipeline educacional, avaliação de especialistas, análise de metadados, análise de rastreabilidade e comparação com pipeline ad hoc.

O FairED-Pipeline deve ser validado não apenas por métricas de fairness, mas também pela capacidade de orientar o processo completo de identificação, análise, mitigação, documentação e monitoramento de vieses.

O SemED-LLM deve ser validado pela estrutura técnica dos módulos e pela orientação metodológica para taxonomia, prompts, validação humana, explicabilidade e governança.

#### 15.8.8 Relatório de validação de framework técnico-metodológico

O relatório deve conter:

definição do framework;

modelo de referência;

arquitetura;

módulos;

artefatos;

metadados;

contratos;

cenário de instanciação;

métricas;

resultados;

avaliação por especialistas;

limitações;

versão revisada.

#### 15.8.9 Síntese

Um framework técnico-metodológico validado deve demonstrar que orienta tanto a construção técnica quanto a condução metodológica da solução.

### 15.9 Validação de plataforma

Uma plataforma é um ambiente computacional integrado que oferece funcionalidades a usuários ou sistemas. Sua validação deve considerar funcionamento técnico, usabilidade, utilidade, desempenho, segurança, navegabilidade e adequação ao público-alvo.

#### 15.9.1 Objetivo da validação de plataforma

Demonstrar que a plataforma funciona corretamente, permite que usuários realizem tarefas previstas, apresenta desempenho adequado, é compreensível, segura e útil ao contexto de aplicação.

#### 15.9.2 Questões de avaliação

As funcionalidades previstas foram implementadas?

Os usuários conseguem realizar as tarefas?

A interface é compreensível?

O tempo de resposta é adequado?

A navegação é eficiente?

O controle de acesso funciona?

A plataforma apoia o objetivo do projeto?

Os usuários consideram a plataforma útil?

#### 15.9.3 Delineamento geral da validação

Etapa 1 — Definir perfis de usuário

Exemplos:

aluno;

docente;

gestor;

pesquisador;

desenvolvedor;

especialista.

Etapa 2 — Definir tarefas representativas

Exemplos:

localizar conceito;

cadastrar fonte;

consultar dashboard;

interpretar mapa;

analisar recomendação;

localizar artefato;

acessar relatório.

Etapa 3 — Preparar protótipo funcional

A plataforma deve permitir a execução mínima das tarefas.

Etapa 4 — Conduzir teste com usuários

Registrar tempo, cliques, erros, dúvidas e sucesso.

Etapa 5 — Aplicar questionário

Avaliar usabilidade, clareza, utilidade e satisfação.

Etapa 6 — Analisar logs

Verificar navegação, falhas e padrões de uso.

Etapa 7 — Revisar a plataforma

Ajustar interface, fluxos, funcionalidades ou documentação.

#### 15.9.4 Métricas para validação de plataforma

Funcionalidade

Funcionalidade = funcionalidades implementadas / funcionalidades previstas

Efetividade

Efetividade = tarefas concluídas com sucesso / tarefas propostas

Eficiência

Eficiência = tempo médio por tarefa

Navegabilidade

Navegabilidade = número médio de cliques por tarefa

Taxa de erro

Taxa de Erro = erros observados / tarefas executadas

Usabilidade

Pode ser medida por SUS ou escala Likert.

Usabilidade = soma das notas dos usuários / pontuação máxima possível

#### 15.9.5 Matriz rigorosa de avaliação de plataforma

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Funcionalidade | funcionalidades implementadas / previstas | checklist | lista de funções | mede completude funcional |

| Efetividade | tarefas concluídas / propostas | teste com usuários | relatório de tarefas | mede sucesso |

| Eficiência | tempo médio | cronometragem | logs | mede rapidez |

| Navegabilidade | cliques por tarefa | log | trilha de navegação | mede facilidade |

| Usabilidade | SUS ou Likert | questionário | respostas | mede experiência |

| Segurança | acessos corretos / tentativas | teste | logs | mede controle |

| Utilidade | nota média | questionário/entrevista | feedback | mede valor percebido |

#### 15.9.6 Delineamento por tipo de plataforma

Plataforma de conhecimento

Aplicável ao UnespDataLens.

| Dimensão | Métrica |

| --- | --- |

| Busca | buscas bem-sucedidas / buscas totais |

| Navegação | cliques por tarefa |

| Cobertura | conceitos documentados / conceitos previstos |

| Utilidade | nota média dos usuários |

Plataforma analítica

Aplicável à MILA-eDU.

| Dimensão | Métrica |

| --- | --- |

| Indicadores | indicadores disponíveis / previstos |

| Decisão | decisões apoiadas / previstas |

| Tempo de análise | tempo médio por cenário |

| Utilidade | nota média dos gestores |

Plataforma geoespacial

Aplicável ao GeoReXAI.

| Dimensão | Métrica |

| --- | --- |

| Mapas | mapas gerados / previstos |

| Interpretação | tarefas corretas / tarefas propostas |

| Clareza visual | nota média dos especialistas |

| Desempenho | tempo de carregamento |

#### 15.9.7 Exemplos de aplicação

O UnespDataLens pode ser validado com alunos e docentes realizando tarefas como localizar conceitos, acessar exemplos e navegar entre módulos.

Uma plataforma MILA-eDU pode ser validada com gestores analisando cenários de evasão.

Uma plataforma GeoReXAI pode ser validada com especialistas interpretando mapas e explicações.

#### 15.9.8 Relatório de validação de plataforma

O relatório deve conter:

perfis de usuário;

tarefas aplicadas;

funcionalidades avaliadas;

métricas;

logs;

resultados de usabilidade;

erros observados;

melhorias propostas.

#### 15.9.9 Síntese

Uma plataforma validada deve demonstrar que funciona, é usável, útil, segura e adequada às tarefas do usuário.

### 15.10 Validação de pipeline

Um pipeline é uma sequência operacional que transforma entradas em saídas. Sua validação deve verificar execução ponta a ponta, qualidade das saídas, rastreabilidade, robustez, monitoramento e reprodutibilidade.

#### 15.10.1 Objetivo da validação de pipeline

Demonstrar que o pipeline executa corretamente suas etapas, produz artefatos válidos, registra metadados e logs, trata falhas, permite rastreabilidade e pode ser reproduzido.

#### 15.10.2 Questões de avaliação

O pipeline executa todas as etapas previstas?

As saídas de cada etapa estão corretas?

Os dados produzidos possuem qualidade adequada?

Os artefatos são rastreáveis?

Os metadados são completos?

O pipeline trata falhas?

O processo pode ser reexecutado?

Há melhoria em relação à execução manual ou ad hoc?

#### 15.10.3 Delineamento geral da validação

Etapa 1 — Definir entrada inicial e saída esperada

Exemplo: dados brutos de AVA como entrada e relatório analítico como saída.

Etapa 2 — Executar pipeline completo

Registrar execução ponta a ponta.

Etapa 3 — Verificar saídas intermediárias

Cada etapa deve gerar artefatos previstos.

Etapa 4 — Avaliar qualidade dos dados

Completude, consistência, validade, unicidade e integridade.

Etapa 5 — Verificar metadados e contratos

Avaliar se campos obrigatórios foram preenchidos e contratos respeitados.

Etapa 6 — Avaliar rastreabilidade

Reconstruir caminho entre entrada e saída.

Etapa 7 — Testar falhas

Simular schema inválido, dado ausente, prompt inválido, camada geográfica com erro ou métrica fora do limite.

Etapa 8 — Reexecutar

Avaliar compatibilidade dos resultados.

#### 15.10.4 Métricas para validação de pipeline

Execução

Execução = etapas executadas / etapas previstas

Sucesso de execução

Sucesso = execuções concluídas / execuções testadas

Cobertura de metadados

Cobertura de Metadados = campos preenchidos / campos obrigatórios

Rastreabilidade

Rastreabilidade = artefatos com linhagem / artefatos totais

Robustez

Robustez = falhas tratadas / falhas simuladas

Reprodutibilidade

Reprodutibilidade = resultados compatíveis / reexecuções

#### 15.10.5 Matriz rigorosa de avaliação de pipeline

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Execução | etapas executadas / previstas | log | registro de execução | mede funcionamento |

| Qualidade | completude/consistência/validade | relatório | métricas de dados | mede confiabilidade |

| Rastreabilidade | artefatos rastreáveis / total | grafo | linhagem | mede auditabilidade |

| Robustez | falhas tratadas / simuladas | teste | relatório de falhas | mede resiliência |

| Reprodutibilidade | reexecuções compatíveis / testadas | reexecução | resultados | mede repetição |

| Contratos | contratos atendidos / definidos | checklist | contratos | mede conformidade |

#### 15.10.6 Delineamento por tipo de pipeline

Pipeline de dados educacionais

Aplicável ao EdmLens.

| Dimensão | Métrica |

| --- | --- |

| Fontes | fontes registradas / fontes utilizadas |

| Qualidade | datasets válidos / datasets gerados |

| Linhagem | artefatos rastreáveis / artefatos totais |

| Catálogo | artefatos catalogados / artefatos gerados |

Pipeline textual com LLM

Aplicável ao SemED-LLM.

| Dimensão | Métrica |

| --- | --- |

| Textos | textos processados / textos recebidos |

| Prompts | prompts registrados / prompts utilizados |

| Respostas | respostas válidas / respostas totais |

| Validação | respostas validadas / amostra |

Pipeline geoespacial

Aplicável ao GeoReXAI.

| Dimensão | Métrica |

| --- | --- |

| Geometrias | geometrias válidas / totais |

| Camadas | camadas processadas / camadas previstas |

| Mapas | mapas gerados / mapas esperados |

| Linhagem | mapas rastreáveis / mapas totais |

#### 15.10.7 Exemplos de aplicação

Um pipeline EdmLens pode ser validado comparando execução ad hoc com execução formalizada.

Um pipeline SemED-LLM pode ser validado verificando se textos, prompts, respostas e validações humanas são registrados.

Um pipeline GeoReXAI pode ser validado verificando se camadas, modelos, explicações e mapas permanecem rastreáveis.

#### 15.10.8 Relatório de validação de pipeline

O relatório deve conter:

entrada e saída esperadas;

etapas executadas;

artefatos gerados;

métricas de qualidade;

logs;

falhas simuladas;

reexecuções;

limitações.

#### 15.10.9 Síntese

Um pipeline validado deve demonstrar que executa, produz artefatos corretos, registra evidências, trata falhas e pode ser reexecutado.

### 15.11 Validação de agente inteligente

Um agente inteligente deve ser validado quanto à qualidade da resposta, segurança, controle de autonomia, rastreabilidade, explicabilidade e adequação ao domínio.

#### 15.11.1 Objetivo da validação de agente inteligente

Demonstrar que o agente executa sua tarefa de forma correta, segura, rastreável, explicável, consistente e compatível com o nível de autonomia permitido.

#### 15.11.2 Questões de avaliação

O agente executa corretamente sua tarefa?

Suas respostas estão aderentes à taxonomia ou regra?

O agente registra prompts, parâmetros, respostas e versões?

O agente respeita limites de autonomia?

Há risco de alucinação ou resposta inválida?

As respostas são úteis para especialistas?

O agente permite validação humana?

O agente é seguro para o domínio?

#### 15.11.3 Delineamento geral da validação

Etapa 1 — Definir tarefa e autonomia

Exemplos:

classificar lacunas;

detectar viés;

monitorar drift;

recomendar conceito;

gerar explicação;

emitir alerta.

Etapa 2 — Definir casos de teste

Casos devem incluir situações normais, ambíguas e críticas.

Etapa 3 — Executar o agente

Registrar entrada, prompt, modelo, parâmetros, saída e justificativa.

Etapa 4 — Comparar com referência

A referência pode ser humana, regra, taxonomia ou baseline.

Etapa 5 — Avaliar desempenho e riscos

Medir acerto, erro, alucinação, segurança e conformidade.

Etapa 6 — Submeter a especialistas

Avaliar utilidade, adequação e explicabilidade.

Etapa 7 — Revisar prompts, regras ou arquitetura

Ajustar agente conforme resultados.

#### 15.11.4 Métricas para validação de agente

Desempenho

Desempenho = respostas corretas / respostas avaliadas

Também pode ser medido por acurácia, precisão, recall ou F1.

Concordância humana

Concordância Humana = respostas concordantes / respostas avaliadas por humanos

Conformidade

Conformidade = respostas no formato esperado / respostas totais

Rastreabilidade

Rastreabilidade = respostas com log completo / respostas totais

Taxa de alucinação

Taxa de Alucinação = respostas incorretas ou inventadas / respostas avaliadas

Controle de autonomia

Controle de Autonomia = ações dentro do nível permitido / ações totais

#### 15.11.5 Matriz rigorosa de avaliação de agente

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Desempenho | F1, acurácia | base rotulada | predições | mede acerto |

| Concordância | concordâncias / total | validação humana | pareceres | mede alinhamento humano |

| Conformidade | respostas válidas / total | validador | logs | mede aderência |

| Rastreabilidade | logs completos / total | análise documental | registros | mede auditabilidade |

| Segurança | violações / execuções | auditoria | relatório | mede risco |

| Utilidade | nota média | especialistas | questionário | mede valor prático |

#### 15.11.6 Delineamento por tipo de agente

Agente de diagnóstico semântico

Aplicável ao SemED-LLM.

| Dimensão | Métrica |

| --- | --- |

| Classificação | F1, precisão, recall |

| Concordância | concordância com docentes |

| Prompt | prompts registrados / utilizados |

| Utilidade | nota média dos docentes |

Agente auditor de fairness

Aplicável ao FairED-Pipeline.

| Dimensão | Métrica |

| --- | --- |

| Detecção | disparidades detectadas / esperadas |

| Métricas | métricas calculadas / previstas |

| Alertas | alertas corretos / alertas emitidos |

| Rastreabilidade | auditorias registradas / executadas |

Agente monitorador

Aplicável ao EdmLens.

| Dimensão | Métrica |

| --- | --- |

| Drift | drifts detectados / drifts simulados |

| Falso positivo | alertas incorretos / alertas totais |

| Tempo de detecção | tempo até alerta |

| Logs | eventos registrados / eventos totais |

#### 15.11.7 Exemplos de aplicação

Um agente SemED-LLM pode ser validado comparando diagnósticos semânticos com avaliações docentes.

Um agente FairED-Pipeline pode ser validado verificando se identifica corretamente disparidades entre grupos.

Um agente EdmLens de monitoramento pode ser validado com cenários simulados de drift e falhas.

#### 15.11.8 Relatório de validação de agente

O relatório deve conter:

tarefa do agente;

nível de autonomia;

casos de teste;

prompts ou regras;

métricas;

comparação com referência;

falhas;

riscos;

ajustes realizados.

#### 15.11.9 Síntese

Um agente validado deve demonstrar acurácia, segurança, rastreabilidade, controle de autonomia e utilidade no domínio.

### 15.12 Validação de artefato computacional

Artefatos computacionais incluem datasets, catálogos, dashboards, templates, relatórios, ontologias, glossários, repositórios, bibliotecas, APIs, guias e especificações.

#### 15.12.1 Objetivo da validação de artefato

Demonstrar que o artefato cumpre sua finalidade, é compreensível, completo, útil, utilizável, documentado e passível de reuso ou avaliação.

#### 15.12.2 Questões de avaliação

O artefato cumpre sua finalidade?

O usuário consegue utilizá-lo?

O artefato é completo?

O artefato é claro?

O artefato está documentado?

O artefato pode ser reutilizado?

O artefato possui limitações conhecidas?

O artefato melhora a execução de uma tarefa?

#### 15.12.3 Delineamento geral da validação

Etapa 1 — Definir finalidade do artefato

Exemplo: documentar, orientar, visualizar, armazenar, consultar, explicar ou avaliar.

Etapa 2 — Definir usuários

Exemplo: alunos, docentes, pesquisadores, gestores, desenvolvedores.

Etapa 3 — Definir tarefa de uso

O artefato deve ser aplicado em uma tarefa.

Etapa 4 — Coletar métricas

Medir completude, clareza, tempo, erro, utilidade ou reuso.

Etapa 5 — Coletar feedback

Usuários ou especialistas avaliam.

Etapa 6 — Revisar artefato

Ajustar conteúdo, estrutura ou interface.

#### 15.12.4 Métricas para validação de artefato

Completude

Completude = itens presentes / itens esperados

Clareza

Clareza = soma das notas dos avaliadores / pontuação máxima possível

Utilidade

Utilidade = soma das notas de utilidade / pontuação máxima possível

Reuso

Reuso = itens reutilizáveis / itens totais

Documentação

Documentação = itens documentados / itens necessários

#### 15.12.5 Matriz rigorosa de avaliação de artefato

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Completude | itens presentes / esperados | checklist | artefato | mede suficiência |

| Clareza | nota média | questionário | respostas | mede compreensão |

| Utilidade | nota média | usuário/especialista | feedback | mede valor |

| Reuso | itens reutilizáveis / totais | análise documental | repositório | mede reutilização |

| Documentação | itens documentados / necessários | checklist | README/documentos | mede apoio ao uso |

#### 15.12.6 Delineamento por tipo de artefato

Dataset

| Dimensão | Métrica |

| --- | --- |

| Completude | campos preenchidos / campos totais |

| Consistência | registros válidos / registros totais |

| Documentação | campos documentados / campos totais |

| Reuso | usuários que conseguem utilizar / usuários avaliados |

Catálogo

| Dimensão | Métrica |

| --- | --- |

| Localização | itens encontrados / itens buscados |

| Tempo | tempo médio de busca |

| Metadados | metadados preenchidos / obrigatórios |

| Utilidade | nota média dos usuários |

Dashboard

| Dimensão | Métrica |

| --- | --- |

| Interpretação | respostas corretas / tarefas |

| Tempo | tempo médio por tarefa |

| Clareza | nota média |

| Utilidade | nota média |

Guia ou template

| Dimensão | Métrica |

| --- | --- |

| Preenchimento | campos preenchidos corretamente / campos totais |

| Clareza | nota média dos usuários |

| Completude | seções preenchidas / seções previstas |

| Utilidade | nota média dos alunos/orientadores |

#### 15.12.7 Exemplos de aplicação

Um catálogo do EdmLens pode ser validado verificando se usuários conseguem localizar datasets, features, modelos e relatórios.

Um dashboard da MILA-eDU pode ser validado por clareza, tempo de interpretação e utilidade para gestores.

Um glossário do UnespDataLens pode ser validado verificando se alunos compreendem conceitos e diferenciam método, técnica, metodologia, arquitetura e framework.

Um template do guia pode ser validado verificando se alunos conseguem preencher corretamente a especificação de seus projetos.

#### 15.12.8 Relatório de validação de artefato

O relatório deve conter:

artefato validado;

finalidade;

usuários;

tarefa de validação;

métricas;

resultados;

feedback;

melhorias realizadas.

#### 15.12.9 Síntese

Um artefato validado deve demonstrar que cumpre sua finalidade, é compreensível, completo, útil e reutilizável.

### 15.13 Validação por especialistas

A avaliação por especialistas pode ser utilizada em diferentes tipos de proposta, especialmente modelos, metodologias, arquiteturas, frameworks e artefatos interpretativos.

#### 15.13.1 Objetivo da validação por especialistas

Coletar avaliação qualificada sobre clareza, coerência, completude, originalidade, aplicabilidade, utilidade, viabilidade e limitações da proposta.

#### 15.13.2 Delineamento geral

Etapa 1 — Definir perfil dos especialistas

Podem participar especialistas em Ciência da Computação, Engenharia de Dados, Educação, IA, governança, domínio de aplicação ou desenvolvimento de software.

Etapa 2 — Preparar material de avaliação

Enviar descrição da proposta, diagramas, modelos, módulos, artefatos e critérios.

Etapa 3 — Definir critérios e escala

Sugere-se escala de 1 a 5.

Etapa 4 — Aplicar questionário ou entrevista

Coletar notas e comentários.

Etapa 5 — Analisar convergências e divergências

Identificar pontos fortes e fragilidades.

Etapa 6 — Revisar proposta

Registrar alterações incorporadas.

#### 15.13.3 Métricas

Nota Média por Critério = soma das notas / número de avaliadores



Sugestões Incorporadas = sugestões incorporadas / sugestões pertinentes

#### 15.13.4 Matriz de avaliação por especialistas

| Critério | Métrica | Instrumento | Evidência | Interpretação |

| --- | --- | --- | --- | --- |

| Clareza | média das notas | questionário | respostas | mede compreensão |

| Coerência | média das notas | questionário | pareceres | mede consistência |

| Completude | média das notas | checklist | avaliação | mede suficiência |

| Aplicabilidade | média das notas | entrevista | comentários | mede viabilidade |

| Utilidade | média das notas | questionário | respostas | mede valor |

| Sugestões | incorporadas / pertinentes | análise qualitativa | versão revisada | mede evolução |

#### 15.13.5 Relatório

O relatório deve conter perfil dos especialistas, critérios, notas, comentários, convergências, divergências e alterações realizadas.

### 15.14 Relatório final de validação

Toda validação deve produzir um relatório estruturado. Esse relatório é uma evidência da maturidade científica da proposta.

#### 15.14.1 Estrutura mínima do relatório

Objeto validado.

Tipo de proposta.

Objetivo da validação.

Questões de avaliação.

Critérios.

Métricas.

Cenário.

Participantes.

Instrumentos.

Procedimento.

Evidências coletadas.

Resultados quantitativos.

Resultados qualitativos.

Interpretação.

Limitações.

Ameaças à validade.

Melhorias propostas.

#### 15.14.2 Modelo geral de matriz de validação

| Questão de avaliação | Critério | Métrica | Instrumento | Evidência | Resultado |

| --- | --- | --- | --- | --- | --- |

| A arquitetura cobre os requisitos? | Cobertura | requisitos atendidos / total | matriz | tabela de mapeamento | percentual |

| O pipeline é rastreável? | Rastreabilidade | relações rastreáveis / esperadas | grafo | linhagem | percentual |

| A plataforma é útil? | Utilidade | nota média | questionário | respostas | média |

| O agente é preciso? | Desempenho | F1-score | base rotulada | predições | valor |

| A metodologia orienta o processo? | Aderência | etapas executadas / previstas | checklist | relatório | percentual |

### 15.15 Síntese

A validação deve ser planejada de acordo com a natureza da proposta. Modelos precisam ser avaliados quanto à representação e aderência. Modelos de referência precisam ser avaliados quanto à completude, generalidade e capacidade de instanciação. Métodos precisam ser avaliados quanto à eficácia em uma tarefa específica. Técnicas precisam ser avaliadas pelo efeito produzido e pelos impactos colaterais. Metodologias precisam ser avaliadas quanto à capacidade de orientar processos. Arquiteturas precisam ser avaliadas por requisitos, componentes, fluxos, dependências, coesão, acoplamento, governança e implementabilidade. Frameworks precisam ser avaliados quanto à aplicabilidade, reuso e capacidade de orientar uma classe de problemas. Frameworks técnico-metodológicos exigem avaliação multicritério, envolvendo modelo de referência, arquitetura, módulos, artefatos, metadados, contratos, governança, rastreabilidade, reprodutibilidade e utilidade. Plataformas precisam ser avaliadas quanto ao funcionamento técnico e à experiência de uso. Pipelines precisam ser avaliados quanto à execução, qualidade, rastreabilidade e reprodutibilidade. Agentes inteligentes precisam ser avaliados quanto à precisão, segurança, rastreabilidade, controle de autonomia e utilidade. Artefatos computacionais precisam ser avaliados quanto à completude, clareza, utilidade e possibilidade de reuso.

Dessa forma, validar uma proposta não significa apenas aplicar um questionário ou apresentar um estudo de caso. Validar significa construir um processo sistemático que articula objeto, critérios, métricas, instrumentos, evidências, análise e revisão. Quanto mais claro for esse delineamento, mais forte será a contribuição científica e computacional da proposta.

### 15.16 Complementos de avaliação científica, comparação e ameaças à validade

A avaliação científica também deve discutir dimensões gerais, comparação com abordagem ad hoc, desenhos de avaliação e ameaças à validade.

Avaliar um framework não é apenas mostrar que o protótipo funcionou. A avaliação deve produzir evidências sobre utilidade, viabilidade, qualidade, rastreabilidade, reprodutibilidade, governança e contribuição científica.

### 15.1 Dimensões de avaliação

| Dimensão | Pergunta | Métrica/evidência | Três exemplos |

| --- | --- | --- | --- |

| Funcional | Executa? | Módulos concluídos. | Ingestão; modelagem; relatório. |

| Técnica | É eficiente? | Tempo, memória, falhas. | Tempo por módulo; uso de RAM; taxa de erro. |

| Qualidade | Dados são confiáveis? | Completude, validade. | Nulos; duplicados; inconsistências. |

| Rastreabilidade | Resultado é auditável? | Cobertura de linhagem. | Dados; modelos; agentes. |

| Reprodutibilidade | Pode repetir? | Reexecução com mesma config. | Docker; seed; versões. |

| Explicabilidade | Resultado é compreensível? | Avaliação de especialistas. | SHAP; justificativa; mapa. |

| Governança | Há controle? | Políticas e logs. | Acesso; validação; auditoria. |

| Utilidade | Ajuda o domínio? | Percepção/efetividade. | Professor; gestor; especialista. |

### 15.2 Comparação com abordagem ad hoc

| Critério | Abordagem ad hoc | Framework formalizado |

| --- | --- | --- |

| Documentação | Incompleta ou dispersa. | Padronizada em módulos e contratos. |

| Rastreabilidade | Baixa ou ausente. | Obrigatória por artefato. |

| Reprodutibilidade | Difícil de repetir. | Configuração, ambiente e versões registrados. |

| Governança | Informal. | Papéis e políticas definidos. |

| Agentes | Caixa-preta. | Entradas, saídas, restrições e logs. |

| Avaliação | Apenas resultado final. | Avaliação multicritério. |

### 15.3 Três desenhos de avaliação

| Desenho | Como funciona | Quando usar |

| --- | --- | --- |

| Estudo de caso único | Aplica o framework em um cenário e coleta evidências. | IC/mestrado com dados reais limitados. |

| Comparação controlada | Compara framework com pipeline ad hoc ou baseline. | Mestrado/doutorado com avaliação técnica. |

| Avaliação com especialistas | Especialistas julgam utilidade, clareza e aplicabilidade. | Quando há forte componente de domínio. |

## 16. Ameaças à validade

A discussão de ameaças à validade mostra maturidade científica. Ela evita conclusões exageradas e explicita limitações do estudo.

| Tipo | Pergunta | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- | --- |

| Interna | O resultado decorre do framework? | Erro de implementação. | Parâmetro inadequado. | Falha de validação. |

| Externa | Generaliza? | Uma única turma. | Uma única instituição. | Um único domínio. |

| Construto | Mede o que promete? | Rastreabilidade medida só por logs. | Utilidade sem especialistas. | Qualidade com poucas métricas. |

| Conclusão | Evidência sustenta conclusão? | Poucos experimentos. | Sem análise estatística. | Sem comparação. |

## 16. Implementação de referência da proposta

A implementação de referência é a materialização mínima, controlada e documentada da proposta. Sua finalidade é demonstrar que a proposta é tecnicamente viável, compreensível, executável ou aplicável. Ela não precisa corresponder a um produto final completo, comercial ou plenamente escalável, mas deve ser suficiente para demonstrar o funcionamento do fluxo principal da proposta, registrando artefatos, metadados, logs, parâmetros, evidências e resultados.

Em uma pesquisa acadêmica, a implementação de referência não deve ser entendida apenas como “fazer um sistema funcionar”. Ela deve demonstrar a relação entre a proposta conceitual e sua aplicação prática. Assim, a implementação deve permitir verificar se os módulos, etapas, métodos, artefatos, contratos e critérios definidos na proposta podem ser efetivamente instanciados.

Uma implementação de referência deve responder às seguintes perguntas:

O que foi implementado?

O que ficou fora do escopo?

Quais módulos, componentes ou etapas foram materializados?

Quais entradas foram utilizadas?

Quais saídas foram produzidas?

Quais artefatos foram gerados?

Quais metadados foram registrados?

Quais logs foram produzidos?

Quais contratos foram verificados?

Quais métricas foram calculadas?

Como o fluxo principal pode ser reproduzido?

Quais limitações permanecem?

A implementação pode assumir diferentes formas, conforme a natureza da proposta: protótipo, pipeline, plataforma, biblioteca, script, serviço, dashboard, agente, catálogo, guia, template, modelo formal, prova de conceito ou repositório técnico-metodológico.

### 16.1 Finalidade da implementação de referência

A implementação de referência possui quatro finalidades principais.

A primeira é demonstrar viabilidade técnica. Isso significa mostrar que a proposta pode ser implementada ou instanciada com tecnologias, dados, artefatos e procedimentos disponíveis.

A segunda é materializar o fluxo principal. Mesmo que nem todos os módulos estejam completos, o fluxo central da proposta deve ser demonstrado. Por exemplo, em um pipeline, deve ser possível partir de uma entrada, executar etapas intermediárias e gerar uma saída. Em uma plataforma, deve ser possível realizar tarefas principais. Em um agente inteligente, deve ser possível receber entrada, processar, gerar resposta e registrar evidências.

A terceira é produzir evidências de validação. A implementação deve gerar logs, métricas, artefatos, relatórios ou registros que possam ser usados na avaliação da proposta.

A quarta é favorecer reprodutibilidade e continuidade. O repositório, a documentação, os exemplos e os scripts devem permitir que outro aluno, pesquisador ou avaliador compreenda como a proposta funciona e como pode ser executada ou adaptada.

### 16.2 Níveis possíveis de implementação

Nem toda proposta precisa ser implementada no mesmo nível. O nível de implementação deve ser compatível com o tipo de pesquisa, maturidade do aluno, tempo disponível, dados acessíveis e contribuição científica pretendida.

| Nível | Característica | Indicado para | Exemplo |

| --- | --- | --- | --- |

| Demonstração conceitual | Modelo, diagrama, matriz, template ou guia validado | IC, propostas conceituais ou metodológicas | Modelo formal + avaliação por especialistas |

| Prova de conceito | Implementação mínima de um fluxo ou componente | IC, Mestrado | Script Python com entrada, processamento e saída |

| Protótipo funcional | Conjunto de módulos executáveis em cenário controlado | Mestrado | Pipeline com dados de exemplo, logs e métricas |

| Plataforma experimental | Interface, banco, API e funcionalidades principais | Mestrado/Doutorado | Plataforma web para consulta, análise ou visualização |

| Framework instanciável | Estrutura modular, documentação, exemplos, templates e execução parcial | Doutorado | Repositório com módulos, contratos, exemplos e avaliação |

| Framework técnico-metodológico completo | Modelo de referência, arquitetura, especificação, artefatos, metadados, validação e reprodutibilidade | Doutorado | Guia + repositório + estudo de caso + métricas |

### 16.3 Estratégias de implementação por tipo de proposta

A implementação deve ser planejada de acordo com a natureza da proposta. A seguir são descritas orientações específicas para cada tipo de contribuição.

### 16.3.1 Implementação de modelo

Quando a proposta é um modelo, a implementação de referência deve demonstrar como o modelo pode ser representado, aplicado e avaliado.

Um modelo pode ser implementado por meio de:

diagrama conceitual;

matriz de conceitos;

ontologia;

grafo de relações;

modelo de dados;

especificação formal;

notebook demonstrativo;

exemplo de aplicação;

ferramenta simples de consulta;

JSON/YAML com os elementos do modelo.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Conceitos | Lista formal dos conceitos do modelo |

| Relações | Relações entre conceitos, variáveis ou entidades |

| Representação | Diagrama, grafo, tabela, ontologia ou arquivo estruturado |

| Exemplo | Aplicação do modelo em um caso concreto |

| Evidências | Matriz conceitual, validação por especialistas ou exemplos resolvidos |

Exemplo aplicado:

No UnespDataLens, um modelo conceitual pode ser implementado como um grafo de conceitos, no qual cada nó representa um conceito, como método, técnica, metodologia, arquitetura, framework, pipeline, modelo e agente. As arestas representam relações, como “é aplicado por”, “compõe”, “depende de”, “exemplifica” ou “é avaliado por”. A implementação pode ser disponibilizada como arquivos Markdown, JSON e páginas navegáveis.

No SemED-LLM, um modelo semântico pode ser implementado como uma taxonomia de lacunas conceituais, contendo categorias, definições, exemplos, critérios de classificação e casos anotados.

### 16.3.2 Implementação de modelo de referência

Quando a proposta é um modelo de referência, a implementação deve demonstrar como seus elementos podem orientar uma instanciação.

Um modelo de referência deve ser implementado por meio de:

documento formal;

matriz de princípios, componentes e artefatos;

templates de instanciação;

exemplos de uso;

checklist de aderência;

repositório com estrutura reutilizável;

pelo menos uma instanciação demonstrativa.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Princípios | Fundamentos que orientam a proposta |

| Componentes | Elementos obrigatórios e opcionais |

| Artefatos | Produtos esperados de cada componente |

| Metadados | Informações mínimas para documentação |

| Contratos | Condições de entrada, saída e qualidade |

| Instanciação | Aplicação do modelo em um cenário |

| Checklist | Verificação de aderência ao modelo |

Exemplo aplicado:

No EdmLens, o modelo de referência pode ser implementado como um conjunto de documentos e templates para especificar fontes, extrações, transformações, integrações, datasets, features, modelos, explicações, logs, metadados, governança, proveniência, monitoramento e catálogo.

Na MILA-eDU, o modelo de referência pode ser implementado por uma sequência de templates que orientem a definição do problema decisório, seleção de indicadores, análise, interpretação, priorização e registro da decisão.

### 16.3.3 Implementação de método

Quando a proposta é um método, a implementação de referência deve demonstrar que o procedimento pode ser executado e avaliado em uma tarefa específica.

Um método deve ser implementado por meio de:

pseudocódigo;

script ou função;

notebook experimental;

conjunto de dados de teste;

baseline comparativo;

parâmetros documentados;

métricas de desempenho;

análise de erro.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Entrada | Dados, parâmetros ou artefatos necessários |

| Processamento | Passos do método |

| Saída | Resultado produzido |

| Baseline | Comparação com método alternativo |

| Métricas | Indicadores de desempenho, qualidade ou utilidade |

| Reprodutibilidade | Código, parâmetros, ambiente e dados documentados |

Exemplo aplicado:

No FairED-Pipeline, um método de mitigação de vieses pode ser implementado como um notebook que recebe um dataset, calcula métricas de fairness antes da mitigação, aplica uma técnica de balanceamento ou reponderação, recalcula as métricas e apresenta o trade-off entre desempenho e equidade.

No SemED-LLM, um método de classificação semântica pode ser implementado com prompts versionados, conjunto de textos anotados, execução com LLM, comparação com classificação docente e cálculo de acurácia, precisão, recall e F1.

### 16.3.4 Implementação de técnica

Quando a proposta envolve uma técnica específica, a implementação deve demonstrar o efeito produzido antes e depois de sua aplicação.

Uma técnica deve ser implementada por meio de:

script ou função isolada;

notebook antes/depois;

conjunto de dados controlado;

parâmetros explícitos;

métricas comparativas;

análise de impacto.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Problema tratado | Desbalanceamento, ausência, ruído, viés, drift etc. |

| Técnica aplicada | Procedimento utilizado |

| Estado anterior | Métricas antes da técnica |

| Estado posterior | Métricas depois da técnica |

| Impacto | Ganho, perda ou trade-off |

| Limite de uso | Quando a técnica não é adequada |

Exemplo aplicado:

No EdmLens, uma técnica de anonimização pode ser implementada recebendo uma base educacional, removendo identificadores diretos, pseudonimizando campos sensíveis, registrando metadados de privacidade e avaliando a manutenção da utilidade analítica.

No GeoReXAI, uma técnica de explicabilidade pode ser implementada gerando mapas de importância e avaliando sua estabilidade e utilidade para especialistas.

### 16.3.5 Implementação de metodologia

Quando a proposta é uma metodologia, a implementação de referência não é necessariamente um software completo. Ela deve demonstrar que a metodologia pode ser aplicada por meio de etapas, templates, instrumentos, registros e artefatos.

Uma metodologia deve ser implementada por meio de:

roteiro de aplicação;

templates por etapa;

checklist de execução;

matriz etapa–entrada–atividade–saída;

estudo de caso;

registros das decisões;

artefatos produzidos;

avaliação dos participantes.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Etapas | Sequência formal da metodologia |

| Entradas | Dados, documentos ou informações necessárias |

| Atividades | O que deve ser feito em cada etapa |

| Saídas | Artefatos produzidos em cada etapa |

| Responsáveis | Quem executa ou valida |

| Evidências | Registros, decisões, relatórios e checklists |

| Aplicação | Caso demonstrativo |

Exemplo aplicado:

Na MILA-eDU, a implementação da metodologia pode ser realizada por meio de um estudo de caso sobre evasão. O pesquisador deve demonstrar a aplicação das etapas: definição do problema, seleção dos indicadores, análise dos fatores associados, interpretação dos resultados, priorização de ações, registro das evidências e avaliação da utilidade pelos gestores.

No FairED-Pipeline, uma metodologia de auditoria de vieses pode ser implementada por meio de templates que orientem a identificação dos grupos, seleção das métricas, cálculo das disparidades, escolha da mitigação, documentação da decisão e monitoramento posterior.

### 16.3.6 Implementação de arquitetura

Quando a proposta é uma arquitetura, a implementação deve demonstrar que seus componentes podem ser instanciados, integrados ou simulados.

Uma arquitetura pode ser implementada por meio de:

prova de conceito;

protótipo parcial;

simulação de fluxo;

repositório modular;

APIs entre componentes;

diagrama executável;

scripts representando módulos;

cenário de uso.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Componentes | Módulos ou serviços principais |

| Relações | Comunicação entre componentes |

| Fluxos | Entrada, processamento e saída |

| Interfaces | APIs, arquivos, contratos ou mensagens |

| Cenários | Casos de uso suportados pela arquitetura |

| Evidências | Logs, artefatos e resultados de execução |

Exemplo aplicado:

No EdmLens, a implementação arquitetural pode demonstrar o fluxo entre fonte de dados, extração, transformação, integração, armazenamento, geração de features, modelagem, explicabilidade, governança, proveniência, monitoramento e catálogo, ainda que em escala reduzida.

No SemED-LLM, a arquitetura pode ser implementada por um protótipo com ingestão textual, anonimização, prompt, chamada ao modelo, classificação, validação docente, explicação e registro de logs.

No UnespDataLens, a arquitetura pode ser implementada como um site navegável com módulos, conceitos, links, glossário, exemplos e busca.

### 16.3.7 Implementação de framework

Quando a proposta é um framework, a implementação de referência deve demonstrar que a estrutura proposta pode orientar uma classe de soluções, e não apenas um exemplo isolado.

Um framework deve ser implementado por meio de:

documentação conceitual;

arquitetura;

módulos;

templates;

exemplos de instanciação;

checklist de aderência;

repositório;

protótipo ou prova de conceito;

estudo de caso.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Classe de problemas | Problemas que o framework orienta |

| Estrutura | Módulos, processos ou etapas |

| Artefatos | Produtos gerados por sua aplicação |

| Instanciação | Aplicação em um cenário |

| Reuso | Elementos reutilizáveis |

| Avaliação | Critérios e métricas de aderência |

Exemplo aplicado:

O EdmLens pode ser implementado como framework por meio de um repositório contendo documentação dos módulos, contratos, metadados, exemplos de pipelines, templates de artefatos, scripts de demonstração e checklist de aderência.

O SemED-LLM pode ser implementado como framework com módulos de ingestão, anonimização, taxonomia, prompting, classificação, validação humana, explicabilidade e logs.

O FairED-Pipeline pode ser implementado como framework por meio de scripts e templates para auditoria de fairness, cálculo de métricas, mitigação, documentação e monitoramento.

### 16.3.8 Implementação de framework técnico-metodológico

Quando a proposta é um framework técnico-metodológico, a implementação deve materializar tanto a dimensão técnica quanto a dimensão metodológica.

A dimensão técnica deve incluir:

módulos;

dados;

artefatos;

contratos;

metadados;

logs;

scripts;

APIs;

exemplos;

execução ou instanciação.

A dimensão metodológica deve incluir:

princípios;

etapas;

orientações de uso;

papéis;

critérios;

métricas;

checklists;

templates;

protocolo de validação;

documentação para reuso.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Modelo de referência | Elementos conceituais do framework |

| Arquitetura | Organização modular |

| Especificação | Descrição detalhada dos módulos |

| Templates | Instrumentos de aplicação |

| Instanciação | Aplicação em um cenário |

| Artefatos | Produtos gerados |

| Metadados | Registros obrigatórios |

| Contratos | Condições de entrada, saída e qualidade |

| Validação | Métricas, instrumentos e evidências |

| Reprodutibilidade | Código, dados, logs, ambiente e documentação |

Exemplo aplicado:

No EdmLens, a implementação como framework técnico-metodológico deve demonstrar um pipeline educacional em escala reduzida, mas completo em termos de documentação. Deve haver fonte de dados, extração, transformação, integração, armazenamento, geração de features, modelo analítico, explicação, registros de governança, proveniência, monitoramento e catálogo. Mesmo que o protótipo seja simples, ele deve demonstrar o fluxo principal e registrar artefatos, metadados, logs e evidências.

No FairED-Pipeline, a implementação técnico-metodológica deve demonstrar não apenas o cálculo das métricas de fairness, mas também a sequência de identificação de grupos, documentação dos riscos, execução de mitigação, comparação antes/depois e registro das decisões.

No SemED-LLM, a implementação técnico-metodológica deve demonstrar a relação entre textos, taxonomia, prompts, LLM, respostas, validação humana, explicações, logs e critérios de segurança.

### 16.3.9 Implementação de plataforma

Quando a proposta é uma plataforma, a implementação deve demonstrar funcionalidades acessíveis ao usuário. A plataforma não precisa estar pronta para produção, mas deve permitir que tarefas representativas sejam executadas.

Uma plataforma deve ser implementada por meio de:

interface;

autenticação, quando necessária;

banco de dados ou arquivos estruturados;

API ou serviços;

páginas, telas ou dashboards;

controle de acesso, quando aplicável;

logs;

tarefas de teste;

documentação de uso.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Usuários | Perfis que utilizarão a plataforma |

| Funcionalidades | Tarefas principais implementadas |

| Interface | Telas, páginas ou dashboards |

| Dados | Fontes, banco ou arquivos |

| Segurança | Acesso, permissões ou restrições |

| Logs | Registro de uso e falhas |

| Avaliação | Tarefas, tempo, erros e feedback |

Exemplo aplicado:

No UnespDataLens, a plataforma pode ser implementada como um site em GitHub Pages com páginas de conceitos, módulos, exemplos, glossário, links internos e busca. A implementação deve demonstrar se um aluno consegue localizar um conceito, entender sua definição, acessar exemplos e navegar para temas relacionados.

Na MILA-eDU, uma plataforma experimental pode permitir a visualização de indicadores de evasão, análise de fatores associados e simulação de cenários de decisão.

No GeoReXAI, uma plataforma pode permitir visualizar mapas, selecionar camadas, interpretar explicações e consultar metadados geoespaciais.

### 16.3.10 Implementação de pipeline

Quando a proposta é um pipeline, a implementação deve demonstrar execução ponta a ponta. O pipeline deve partir de uma entrada, executar etapas intermediárias e produzir uma saída rastreável.

Um pipeline deve ser implementado por meio de:

scripts ou notebooks;

diretórios de entrada e saída;

logs;

artefatos intermediários;

metadados;

contratos;

testes;

instruções de reexecução.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Entrada | Dados brutos ou artefatos iniciais |

| Etapas | Processos intermediários |

| Saídas | Artefatos finais |

| Logs | Registro de execução |

| Metadados | Documentação dos artefatos |

| Erros | Tratamento de falhas |

| Reexecução | Possibilidade de reproduzir o fluxo |

Exemplo aplicado:

No EdmLens, um pipeline de dados educacionais pode receber dados acadêmicos, executar limpeza, transformação, integração, geração de features, modelagem, explicabilidade e catalogação. A implementação deve salvar datasets intermediários, logs de execução, metadados e relatório final.

No SemED-LLM, o pipeline deve receber textos, anonimizar, aplicar prompt, obter classificação, registrar resposta, validar com docente e gerar relatório.

No GeoReXAI, o pipeline deve receber camadas geoespaciais, validar geometrias, integrar atributos, treinar modelo, gerar explicações e produzir mapas interpretáveis.

### 16.3.11 Implementação de agente inteligente

Quando a proposta envolve agente inteligente, a implementação deve demonstrar tarefa, autonomia, entrada, saída, logs, validação e limites de ação.

Um agente inteligente deve ser implementado por meio de:

definição da tarefa;

prompts ou regras;

base de casos de teste;

execução controlada;

logs;

registro de parâmetros;

validação humana;

avaliação de riscos;

limites de autonomia.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Tarefa | O que o agente deve executar |

| Entrada | Texto, dados, contexto ou artefato |

| Processamento | Prompt, regra, modelo ou ferramenta |

| Saída | Resposta, alerta, diagnóstico ou recomendação |

| Autonomia | O que pode e não pode fazer |

| Logs | Registro de entrada, modelo, resposta e versão |

| Validação | Comparação com referência humana ou regra |

| Segurança | Bloqueios, restrições e revisão humana |

Exemplo aplicado:

No SemED-LLM, um agente de diagnóstico semântico deve receber interações textuais, classificar lacunas conceituais, justificar a classificação, registrar prompt e resposta, e permitir validação docente.

No FairED-Pipeline, um agente auditor pode calcular métricas de fairness, identificar disparidades, gerar alertas e registrar evidências.

No EdmLens, um agente monitorador pode acompanhar métricas de qualidade, drift e falhas no pipeline, emitindo alertas documentados.

### 16.3.12 Implementação de artefato computacional

Quando a proposta é um artefato computacional específico, a implementação deve demonstrar sua finalidade, uso e avaliação.

Artefatos computacionais podem incluir:

dataset;

catálogo;

dashboard;

glossário;

template;

guia;

ontologia;

API;

relatório;

biblioteca;

repositório.

A implementação deve conter:

| Elemento | O que demonstrar |

| --- | --- |

| Finalidade | Para que o artefato existe |

| Usuário | Quem utiliza |

| Estrutura | Como está organizado |

| Uso | Como aplicar ou consultar |

| Evidência | O que demonstra sua utilidade |

| Avaliação | Como será validado |

| Reuso | Como pode ser reaproveitado |

Exemplo aplicado:

Um glossário do UnespDataLens pode ser implementado como páginas Markdown com definição, exemplos, relações e links.

Um catálogo do EdmLens pode ser implementado como tabela ou interface com datasets, features, modelos, relatórios, metadados e status de uso.

Um dashboard da MILA-eDU pode ser implementado com indicadores, filtros, visualizações e interpretações.

Um template do guia pode ser implementado como documento preenchível para especificação de módulos, métodos ou artefatos.

### 16.4 Manifesto do framework e estratégias complementares de implementação

Além da implementação de referência, recomenda-se registrar um manifesto do framework e explicitar as estratégias de implementação adotadas.

### 13.2 Três estratégias de implementação

| Estratégia | Quando usar | Exemplo |

| --- | --- | --- |

| Protótipo simples | IC ou prova de conceito. | Python scripts + CSV + JSON. |

| Pipeline estruturado | Mestrado. | Python + PostgreSQL + MLflow + testes. |

| Framework robusto | Doutorado. | Orquestração + APIs + catálogo + agentes. |

### 13.3 Manifesto do framework

framework:

nome: FrameworkExemplo

versao: 1.0

dominio: educacao

modulos:

- id: M1

nome: Fontes

obrigatorio: true

- id: M2

nome: Extracao

obrigatorio: true

- id: M3

nome: Transformacao

obrigatorio: true

agentes:

- id: A1

nome: Agente_Validador

nivel_autonomia: 1

rastreabilidade:

registrar_dados: true

registrar_processos: true

registrar_agentes: true

governanca:

anonimizar_dados: true

exigir_validacao_humana: true

## 17. Estrutura de repositório da proposta

Toda proposta deve produzir documentação adequada ao seu tipo. O repositório é parte da implementação de referência, pois organiza código, documentos, dados, exemplos, templates, artefatos, logs e evidências.

O repositório não deve ser apenas um local para guardar arquivos. Ele deve demonstrar organização, rastreabilidade e possibilidade de reprodução.

### 17.1 Estrutura geral recomendada

nome-da-proposta/

├── README.md

├── docs/

│   ├── 01-visao-geral.md

│   ├── 02-conceitos.md

│   ├── 03-modelo-de-referencia.md

│   ├── 04-arquitetura.md

│   ├── 05-modulos-ou-etapas.md

│   ├── 06-metadados.md

│   ├── 07-contratos.md

│   ├── 08-governanca.md

│   ├── 09-validacao.md

│   ├── 10-exemplos.md

│   └── figuras/

├── templates/

├── examples/

├── configs/

├── data/

│   ├── raw/

│   ├── processed/

│   └── sample/

├── src/

├── notebooks/

├── tests/

├── outputs/

│   ├── logs/

│   ├── reports/

│   ├── metrics/

│   └── artifacts/

└── LICENSE



### 17.2 Função de cada diretório

| Diretório | Função |

| --- | --- |

| README.md | Apresentar a proposta, objetivo, instalação e execução |

| docs/ | Documentação conceitual, técnica e metodológica |

| templates/ | Modelos de preenchimento para módulos, artefatos, metadados e validação |

| examples/ | Exemplos de aplicação ou instanciação |

| configs/ | Arquivos de configuração, parâmetros, prompts ou regras |

| data/ | Dados de exemplo, amostras ou dados processados |

| src/ | Código-fonte da implementação |

| notebooks/ | Experimentos, análises e demonstrações |

| tests/ | Testes automatizados ou scripts de verificação |

| outputs/ | Resultados, logs, relatórios, métricas e artefatos gerados |

| LICENSE | Licença de uso |

### 17.3 Estrutura mínima por tipo de proposta

#### Modelo ou modelo de referência

nome-do-modelo/

├── README.md

├── docs/

│   ├── definicao.md

│   ├── conceitos.md

│   ├── relacoes.md

│   ├── matriz-conceitual.md

│   └── validacao.md

├── examples/

│   └── exemplo-aplicacao.md

├── templates/

│   └── matriz-validacao.xlsx

└── outputs/

└── relatorio-validacao.md

#### Método ou técnica

nome-do-metodo/

├── README.md

├── docs/

│   ├── descricao-metodo.md

│   ├── entradas-saidas.md

│   └── validacao.md

├── src/

│   └── metodo.py

├── notebooks/

│   └── experimento.ipynb

├── data/

│   └── sample/

├── outputs/

│   ├── metrics/

│   └── reports/

└── tests/

#### Metodologia

nome-da-metodologia/

├── README.md

├── docs/

│   ├── etapas.md

│   ├── papeis.md

│   ├── instrumentos.md

│   ├── validacao.md

│   └── estudo-de-caso.md

├── templates/

│   ├── etapa-template.md

│   ├── checklist.md

│   └── matriz-etapa-saida.xlsx

├── examples/

│   └── caso-aplicado.md

└── outputs/

└── relatorio-aplicacao.md

#### Arquitetura, framework ou framework técnico-metodológico

nome-do-framework/

├── README.md

├── docs/

│   ├── 01-visao-geral.md

│   ├── 02-modelo-referencia.md

│   ├── 03-arquitetura.md

│   ├── 04-modulos.md

│   ├── 05-artefatos.md

│   ├── 06-metadados.md

│   ├── 07-contratos.md

│   ├── 08-governanca.md

│   ├── 09-validacao.md

│   └── 10-instanciacao.md

├── templates/

├── examples/

├── configs/

├── src/

├── tests/

└── outputs/

├── logs/

├── metrics/

├── reports/

└── artifacts/

#### Plataforma

nome-da-plataforma/

├── README.md

├── docs/

│   ├── requisitos.md

│   ├── arquitetura.md

│   ├── usuarios.md

│   ├── tarefas-validacao.md

│   └── manual-uso.md

├── backend/

├── frontend/

├── database/

├── tests/

├── logs/

└── outputs/

└── relatorio-usabilidade.md

#### Pipeline

nome-do-pipeline/

├── README.md

├── docs/

│   ├── fluxo.md

│   ├── etapas.md

│   ├── contratos.md

│   ├── metadados.md

│   └── validacao.md

├── data/

│   ├── raw/

│   ├── processed/

│   └── sample/

├── src/

│   ├── extract.py

│   ├── transform.py

│   ├── load.py

│   └── validate.py

├── configs/

├── outputs/

│   ├── logs/

│   ├── metrics/

│   ├── artifacts/

│   └── reports/

└── tests/

#### Agente inteligente

nome-do-agente/

├── README.md

├── docs/

│   ├── tarefa.md

│   ├── autonomia.md

│   ├── riscos.md

│   ├── validacao.md

│   └── governanca.md

├── prompts/

├── cases/

├── src/

├── outputs/

│   ├── logs/

│   ├── responses/

│   ├── metrics/

│   └── reports/

└── tests/



### 17.4 Testes da proposta e exemplos de verificação

Testes ajudam a demonstrar que módulos, contratos, dados, agentes e pipelines executam corretamente e produzem evidências de confiabilidade.

Testes devem ser planejados como parte da implementação. Um framework acadêmico ganha rigor quando seus módulos possuem testes de funcionamento, integração, qualidade, rastreabilidade e agentes.

| Tipo de teste | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- |

| Schema | Campos obrigatórios. | Tipos válidos. | Chaves presentes. |

| Qualidade | Completude. | Duplicidade. | Consistência. |

| Transformação | Regra aplicada. | Anonimização. | Conversão de tipo. |

| Linhagem | Origem registrada. | Atividade registrada. | Agente registrado. |

| Modelo | Métrica mínima. | Seed controlada. | Hiperparâmetros salvos. |

| Agente | Não viola restrição. | Registra prompt. | Exige validação. |

| Integração | Módulos em sequência. | Contratos respeitados. | Saídas disponíveis. |

### 14.1 Exemplos de testes em Python

def test_schema_campos_obrigatorios(dataset):

campos = {"id_estudante", "disciplina", "atividade", "data"}

assert campos.issubset(set(dataset.columns))

def test_linhagem_registrada(resultado_modulo):

assert resultado_modulo["linhagem"] is not None

assert resultado_modulo["linhagem"]["dataset_origem"] is not None

def test_agente_nao_executa_acao_proibida(acao_agente):

assert acao_agente["atribuiu_nota"] is False

assert acao_agente["validacao_humana"] is True

### 17.5 GitHub, página do guia e publicação do material

Recomenda-se transformar este guia em um repositório GitHub com uma página publicada via GitHub Pages. Isso facilita atualização contínua, distribuição aos alunos, versionamento, criação de issues, exemplos de código, templates preenchíveis e reuso em diferentes orientações.

### 20.1 Estrutura recomendada para o repositório do guia

guia-frameworks-pipelines-dados/

├── README.md

├── docs/

│   ├── index.md

│   ├── 01-conceitos.md

│   ├── 02-fundamentacao.md

│   ├── 03-especificacao-framework.md

│   ├── 04-modulos-contratos.md

│   ├── 05-metadados-rastreabilidade.md

│   ├── 06-governanca-reprodutibilidade.md

│   ├── 07-agentes-inteligentes.md

│   ├── 08-implementacao.md

│   ├── 09-avaliacao.md

│   └── 10-templates.md

├── templates/

│   ├── template_modulo.md

│   ├── template_agente.md

│   ├── template_contrato.json

│   └── template_pipeline.yaml

├── examples/

│   ├── exemplo_edmlens_t/

│   ├── exemplo_semed_llm/

│   └── exemplo_georexai/

├── mkdocs.yml

└── LICENSE

### 20.2 Vantagens do GitHub Pages

O guia fica acessível como página web para todos os alunos.

Cada atualização fica versionada.

Os alunos podem baixar templates e exemplos.

É possível criar exemplos por projeto: EdmLens-T, SemED-LLM, GeoReXAI etc.

Pode-se usar issues para dúvidas frequentes e melhorias.

O guia pode evoluir como material didático permanente.

## 18. Checklist final de implementação, documentação e formalização

Antes de considerar a proposta madura, o aluno ou pesquisador deve verificar se a proposta está suficientemente formalizada, implementada, documentada e validável.

O checklist a seguir não deve ser tratado apenas como uma lista de conferência superficial. Ele deve orientar a revisão final da proposta, do repositório, dos artefatos e da seção de metodologia ou validação.

### 18.1 Identificação da contribuição

| Pergunta | Evidência esperada |

| --- | --- |

| O tipo de contribuição foi definido? | Declaração explícita: modelo, método, metodologia, arquitetura, framework, plataforma, pipeline, agente ou artefato |

| A lacuna está clara? | Seção de problema e lacuna |

| O problema é relevante? | Justificativa científica, técnica ou aplicada |

| A proposta tem nome, escopo e objetivo? | Título, objetivo geral e objetivos específicos |

| A contribuição para Ciência da Computação está explícita? | Texto de contribuição técnica, metodológica ou científica |

### 18.2 Formalização conceitual

| Pergunta | Evidência esperada |

| --- | --- |

| Os conceitos centrais estão definidos? | Glossário ou seção conceitual |

| Há distinção entre método, técnica, metodologia, arquitetura e framework? | Definições no texto |

| O domínio foi delimitado? | Descrição do contexto de aplicação |

| Há exemplos de uso dos conceitos? | Quadros ou exemplos aplicados |

| Há relação entre conceitos? | Diagrama, matriz ou mapa conceitual |

### 18.3 Estrutura da proposta

| Pergunta | Evidência esperada |

| --- | --- |

| Existe modelo de referência, quando aplicável? | Documento ou seção específica |

| Existe arquitetura, quando aplicável? | Diagrama e descrição das visões |

| Existem módulos, etapas ou componentes? | Lista e especificação |

| As responsabilidades estão claras? | Tabela de responsabilidades |

| As entradas e saídas estão definidas? | Contratos ou especificação dos módulos |

| As dependências estão claras? | Diagrama ou matriz de dependências |

### 18.4 Implementação de referência

| Pergunta | Evidência esperada |

| --- | --- |

| O fluxo principal foi implementado ou demonstrado? | Protótipo, notebook, prova de conceito ou estudo de caso |

| A entrada inicial está definida? | Dataset, texto, prompt, camada, cenário ou documento |

| As saídas foram produzidas? | Relatórios, classificações, mapas, logs, datasets, dashboards |

| Há artefatos intermediários? | Arquivos, tabelas, modelos, explicações ou registros |

| A implementação registra logs? | Arquivos de log ou registros de execução |

| A implementação registra metadados? | JSON, YAML, tabela ou catálogo |

| A implementação pode ser reexecutada? | README, scripts, ambiente e instruções |

### 18.5 Artefatos, metadados e contratos

| Pergunta | Evidência esperada |

| --- | --- |

| Os artefatos foram definidos? | Lista de artefatos |

| Os artefatos foram produzidos? | Pasta outputs/ ou reports/ |

| Os metadados foram definidos? | Modelo de metadados |

| Os metadados foram preenchidos? | Arquivos JSON/YAML/tabelas |

| Existem contratos? | Contratos de entrada, saída, qualidade e erro |

| Os contratos foram testados? | Logs, testes ou relatório de validação |

| Há versionamento? | Controle de versões, Git, tags ou changelog |

### 18.6 Governança, segurança e ética

| Pergunta | Evidência esperada |

| --- | --- |

| A governança foi tratada? | Políticas, papéis e responsabilidades |

| Há controle de acesso, quando necessário? | Autenticação, permissões ou restrições |

| Dados sensíveis foram identificados? | Classificação de sensibilidade |

| Há anonimização ou pseudonimização, quando aplicável? | Registro do procedimento |

| Há logs de ações relevantes? | Arquivos de auditoria |

| Há limites de uso da proposta? | Seção de riscos e restrições |

| Há validação humana em decisões sensíveis? | Registro de aprovação ou revisão |

### 18.7 Qualidade, rastreabilidade e reprodutibilidade

| Pergunta | Evidência esperada |

| --- | --- |

| Existem critérios de qualidade? | Métricas e limites definidos |

| A qualidade dos dados ou artefatos foi avaliada? | Relatório de qualidade |

| A proveniência foi tratada? | Grafo, matriz ou tabela de linhagem |

| É possível reconstruir o caminho entrada → processo → saída? | Registro de rastreabilidade |

| Há estratégia de monitoramento? | Métricas, alertas ou logs |

| Há estratégia de reprodutibilidade? | README, ambiente, dependências, parâmetros e seeds |

| Resultados podem ser reexecutados? | Scripts e instruções |

### 18.8 Validação e avaliação

| Pergunta | Evidência esperada |

| --- | --- |

| Há forma de validação? | Protocolo de validação |

| Há questões de avaliação? | Lista de perguntas avaliativas |

| Há critérios definidos? | Tabela de critérios |

| Há métricas? | Fórmulas, indicadores ou escalas |

| Há instrumentos? | Checklist, questionário, entrevista, logs ou testes |

| Há evidências esperadas? | Lista de artefatos e registros |

| Há relatório de validação? | Documento de resultados |

| Há análise de limitações? | Ameaças à validade e restrições |

### 18.9 Repositório e documentação

| Pergunta | Evidência esperada |

| --- | --- |

| Existe repositório organizado? | Estrutura de pastas |

| Existe README? | Instruções iniciais |

| Há documentação conceitual? | Pasta docs/ |

| Há documentação técnica? | Instalação, execução, parâmetros |

| Há exemplos? | Pasta examples/ |

| Há templates? | Pasta templates/ |

| Há outputs? | Logs, métricas, relatórios e artefatos |

| Há licença? | Arquivo LICENSE |

| Há instrução de reprodução? | Passo a passo de execução |

### 18.10 Checklist por tipo de proposta

#### Modelo

Os conceitos estão definidos?

As relações foram especificadas?

Há diagrama ou matriz conceitual?

Há exemplos de aplicação?

O modelo foi avaliado por especialistas ou aplicado em casos?

Há registro de revisão?

#### Modelo de referência

Os princípios foram definidos?

Os componentes essenciais foram definidos?

Os artefatos esperados foram definidos?

Os metadados e contratos foram previstos?

Há checklist de aderência?

O modelo foi instanciado em pelo menos um cenário?

#### Método

A tarefa do método está clara?

Entradas e saídas foram definidas?

Há pseudocódigo ou implementação?

Há baseline?

Há métricas?

Há análise de erro?

Há parâmetros documentados?

#### Técnica

O problema operacional tratado está claro?

A técnica foi justificada?

Há comparação antes/depois?

Há parâmetros registrados?

O impacto foi medido?

Há análise de efeitos colaterais?

#### Metodologia

As etapas foram formalizadas?

Cada etapa possui entrada, atividade, saída e responsável?

Há templates ou instrumentos?

A metodologia foi aplicada em um caso?

As saídas foram produzidas?

Houve feedback de usuários ou especialistas?

#### Arquitetura

Os requisitos arquiteturais foram definidos?

Os componentes foram descritos?

As relações foram representadas?

Há múltiplas visões arquiteturais?

Há matriz requisito-componente?

Há cenário de uso ou prova de conceito?

#### Framework

A classe de problemas está clara?

Os módulos ou componentes foram definidos?

Há artefatos esperados?

Há critérios de aderência?

Há exemplo de instanciação?

Há avaliação de reuso ou aplicabilidade?

#### Framework técnico-metodológico

Há modelo de referência?

Há arquitetura?

Há módulos especificados?

Há artefatos, metadados e contratos?

Há diretrizes de aplicação?

Há implementação de referência?

Há protocolo de validação?

Há evidência de reprodutibilidade?

#### Plataforma

Os perfis de usuários foram definidos?

As funcionalidades principais foram implementadas?

Há interface funcional?

Há controle de acesso, quando necessário?

Há logs?

Há teste com usuários?

Há avaliação de usabilidade?

#### Pipeline

A entrada e a saída foram definidas?

As etapas foram implementadas?

Há logs de execução?

Há artefatos intermediários?

Há metadados?

Há tratamento de falhas?

Há possibilidade de reexecução?

#### Agente inteligente

A tarefa do agente está definida?

O nível de autonomia está delimitado?

Há prompts, regras ou modelo documentado?

Há logs de entrada, resposta e parâmetros?

Há casos de teste?

Há validação humana?

Há análise de risco?

#### Artefato computacional

A finalidade está clara?

O usuário foi definido?

O artefato está documentado?

O artefato foi aplicado em uma tarefa?

A utilidade foi avaliada?

Há possibilidade de reuso?

### 18.11 Síntese da implementação e formalização

Uma proposta computacional está madura quando não depende apenas de uma descrição textual ou de uma figura conceitual. Ela precisa demonstrar, mesmo que em escala reduzida, como seu fluxo principal funciona, quais artefatos são produzidos, quais metadados são registrados, quais logs são gerados, quais contratos são atendidos, quais métricas são calculadas e quais evidências sustentam sua validação.

A implementação de referência deve ser compatível com a natureza da contribuição. Um modelo deve ser representado e aplicado. Um método deve ser executado e comparado. Uma metodologia deve ser aplicada e produzir artefatos por etapa. Uma arquitetura deve ser instanciada ou demonstrada por prova de conceito. Um framework deve orientar uma classe de problemas e gerar artefatos reutilizáveis. Um framework técnico-metodológico deve combinar implementação técnica e orientação metodológica. Uma plataforma deve permitir tarefas reais de usuários. Um pipeline deve executar ponta a ponta. Um agente deve operar com rastreabilidade, limites de autonomia e validação. Um artefato deve cumprir sua finalidade e demonstrar utilidade.

Dessa forma, a implementação de referência, o repositório e o checklist final formam o elo entre a proposta científica e sua demonstração prática. Eles permitem que a banca, os avaliadores, os orientadores e outros pesquisadores compreendam não apenas o que foi proposto, mas também como a proposta pode ser aplicada, avaliada, reproduzida e evoluída.

### 18.12 Templates preenchíveis para o aluno

Os templates a seguir ajudam o aluno a transformar conceitos, módulos, agentes e avaliação em instrumentos preenchíveis, reduzindo ambiguidades na especificação.

### 18.1 Template: identificação do artefato

| Campo | Preencher |

| --- | --- |

| Nome do framework |  |

| Domínio |  |

| Classe de problema |  |

| Lacuna principal |  |

| Objetivo geral |  |

| Tipo de artefato | Framework / arquitetura / método / protótipo |

| Usuários |  |

| Estudo de caso |  |

| Estratégia de avaliação |  |

### 18.2 Template: especificação de módulo

| Campo | Preencher |

| --- | --- |

| Nome do módulo |  |

| Objetivo |  |

| Responsabilidade |  |

| Fora do escopo |  |

| Entradas |  |

| Processamento |  |

| Saídas |  |

| Artefatos |  |

| Metadados |  |

| Critérios de qualidade |  |

| Erros previstos |  |

| Critérios de avaliação |  |

| Exemplo de implementação |  |

### 18.3 Template: agente inteligente

| Campo | Preencher |

| --- | --- |

| Nome do agente |  |

| Tipo | Validador / classificador / explicativo / recomendador / monitorador / orquestrador |

| Objetivo |  |

| Entradas |  |

| Saídas |  |

| Nível de autonomia | 0 a 5 |

| Restrições |  |

| Logs obrigatórios |  |

| Validação humana | Sim/Não/Quando |

| Métricas de avaliação |  |

### 18.4 Template: plano de avaliação

| Dimensão | Métrica/evidência | Procedimento | Resultado esperado |

| --- | --- | --- | --- |

| Funcional |  |  |  |

| Técnica |  |  |  |

| Qualidade dos dados |  |  |  |

| Rastreabilidade |  |  |  |

| Reprodutibilidade |  |  |  |

| Governança |  |  |  |

| Agentes |  |  |  |

| Utilidade no domínio |  |  |  |

### 18.13 Estrutura sugerida para dissertação, tese ou projeto

| Capítulo | Conteúdo mínimo |

| --- | --- |

| 1. Introdução | Contexto, problema, lacuna, objetivos, RQs, justificativa e contribuições. |

| 2. Fundamentação teórica | Domínio, frameworks, arquiteturas, pipelines, governança, proveniência, reprodutibilidade, agentes e trabalhos relacionados. |

| 3. Metodologia | DSR, estudo de caso, experimento, etapas, dados, avaliação e ameaças à validade. |

| 4. Framework proposto | Princípios, stakeholders, visões, módulos, contratos, metadados, governança, rastreabilidade e agentes. |

| 5. Implementação de referência | Tecnologias, repositório, módulos implementados, testes e execução. |

| 6. Estudo de caso e avaliação | Cenários, métricas, resultados, discussão e comparação. |

| 7. Conclusão | Síntese, contribuições, limitações e trabalhos futuros. |

### 18.14 Contribuição científica

A contribuição científica deve emergir da relação entre lacuna, artefato e avaliação. Não é necessário dizer artificialmente que o trabalho é inovador; é melhor demonstrar a contribuição por meio da estrutura proposta e das evidências produzidas.

| Tipo de contribuição | Exemplo 1 | Exemplo 2 | Exemplo 3 |

| --- | --- | --- | --- |

| Conceitual | Modelo de lacunas conceituais. | Modelo de metadados educacionais. | Modelo de agentes em pipeline. |

| Metodológica | Roteiro para formalizar frameworks. | Processo de validação de LLM. | Método de avaliação de rastreabilidade. |

| Arquitetural | Arquitetura modular com governança. | Arquitetura agentic rastreável. | Arquitetura geoespacial XAI. |

| Técnica | Protótipo implementado. | Módulo de linhagem. | Agente validador. |

| Experimental | Estudo de caso. | Comparação com baseline. | Avaliação com especialistas. |

| Instrumental | Repositório, templates e documentação. | Dataset anonimizado. | Catálogo de artefatos. |

### 17.1 Exemplo de texto de contribuição

Este trabalho contribui ao propor uma estrutura técnico-metodológica para construção de pipelines educacionais rastreáveis e reprodutíveis, integrando módulos de ingestão, transformação, modelagem, explicabilidade, governança e proveniência. A contribuição é demonstrada por meio de uma implementação de referência e de um estudo de caso no qual são avaliadas a execução funcional do pipeline, a qualidade dos dados, a cobertura de rastreabilidade e a capacidade de reprodução dos resultados.

## 19. Síntese final

Este guia técnico-metodológico foi elaborado para apoiar a formalização de propostas computacionais em diferentes níveis de maturidade, desde projetos de Iniciação Científica até teses de Doutorado. Ele diferencia conceitos fundamentais, como modelo, modelo de referência, método, técnica, metodologia, arquitetura, pipeline, plataforma, framework, framework técnico-metodológico, agente inteligente e artefato computacional.

Sua principal contribuição é oferecer uma estrutura para que propostas acadêmicas deixem de ser apenas ideias ou figuras conceituais e passem a ser artefatos científicos formalizados, implementáveis, documentáveis, avaliáveis, rastreáveis e reprodutíveis.

Ao incorporar exemplos de projetos como EdmLens, MILA-eDU, UnespDataLens, SemED-LLM, FairED-Pipeline, GeoReXAI e EduPipeX, o guia demonstra que uma mesma estrutura técnico-metodológica pode apoiar propostas distintas, respeitando suas especificidades.

A validação ocupa papel central no guia. Cada tipo de proposta deve ser avaliado de acordo com sua natureza: modelos devem ser avaliados quanto à representação e aderência; métodos quanto à efetividade; técnicas quanto ao efeito produzido; metodologias quanto à capacidade de orientar processos; arquiteturas quanto à organização e completude; frameworks quanto à aplicabilidade e reuso; frameworks técnico-metodológicos quanto à integração entre fundamentos, módulos, artefatos, metadados, contratos, governança e rastreabilidade; plataformas quanto ao funcionamento e à experiência do usuário; pipelines quanto à execução e qualidade; agentes quanto à precisão, segurança e controle de autonomia; e artefatos quanto à utilidade, completude e possibilidade de reuso.

Dessa forma, o guia busca fortalecer a qualidade científica e técnica das propostas desenvolvidas em Ciência da Computação, oferecendo uma base comum para conceber, formalizar, implementar, validar e evoluir artefatos computacionais em diferentes domínios.

## 20. Referências-base

As referências-base abaixo devem ser usadas para fundamentar propostas que envolvem design science, arquitetura, mineração de dados, governança, proveniência, FAIR, MLOps/DataOps, IA responsável e avaliação de artefatos computacionais.

Hevner, A. R.; March, S. T.; Park, J.; Ram, S. Design Science in Information Systems Research. MIS Quarterly, 2004.

Peffers, K.; Tuunanen, T.; Rothenberger, M. A.; Chatterjee, S. A Design Science Research Methodology for Information Systems Research. Journal of Management Information Systems, 2007.

Sein, M. K.; Henfridsson, O.; Purao, S.; Rossi, M.; Lindgren, R. Action Design Research. MIS Quarterly, 2011.

ISO/IEC/IEEE 42010. Software, systems and enterprise — Architecture description.

Chapman, P. et al. CRISP-DM 1.0: Step-by-step data mining guide. SPSS, 2000.

Studer, S. et al. Towards CRISP-ML(Q): A Machine Learning Process Model with Quality Assurance Methodology. 2020.

W3C. PROV-DM: The PROV Data Model. 2013.

W3C. PROV-O: The PROV Ontology. 2013.

Wilkinson, M. D. et al. The FAIR Guiding Principles for scientific data management and stewardship. Scientific Data, 2016.

NIST. Artificial Intelligence Risk Management Framework (AI RMF 1.0). 2023.

DataOps Manifesto. DataOps Principles.

Yin, R. K. Case Study Research and Applications.

Wohlin, C. et al. Experimentation in Software Engineering.

Bass, L.; Clements, P.; Kazman, R. Software Architecture in Practice.

Fowler, M. Patterns of Enterprise Application Architecture.

Humble, J.; Farley, D. Continuous Delivery.

Sculley, D. et al. Hidden Technical Debt in Machine Learning Systems.

Gebru, T. et al. Datasheets for Datasets.

Mitchell, M. et al. Model Cards for Model Reporting.

Souza, R. et al. PROV-AGENT: Unified Provenance for Tracking AI Agent Interactions in Agentic Workflows, 2025.
