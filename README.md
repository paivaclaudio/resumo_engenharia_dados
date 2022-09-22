# O Papel dos Bancos de Dados SQL e NoSQL na Engenharia de Dados

## Contexto geral sobre o uso banco de dados na atualidade

Para fazer uso da ferramenta certa para resolver o problema que está sendo tratado é preciso entender bem quais funcionalidades são oferecidas por cada ferramenta.
Também é preciso pensar no custo de manutenção da ferramenta adotada.

### • O que é Engenharia de Dados?

A Engenharia de Dados é a área de estudo responsável por processar e transformar os dados brutos de uma empresa, e a partir daí, disponibilizá-los, garantindo que outros profissionais possam utilizá-los para diferentes finalidades.

### •  Qual a diferença entre Engenharia de Dados e Ciência de Dados?

**Engenheiro de Dados:** é o responsável pelas etapas de preparação dos dados. Suas habilidades são concentradas em linguagens de programação e construção de sistemas.

**Cientista de Dados:** busca analisar essas informações, e a partir daí, gerar insights e conclusões que possam ser utilizadas para o negócio. Para isso, ele precisa ter domínio de matemática e estatística, além de habilidades analíticas.

### • O que é SQL e NoSQL

**BD relacional:** é um tipo de BD onde os dados são armazenados e precisam ter relacionamento entre si. É usado para quando se tem um schema de dados rígido e bem definido. Quando se conhece antes o tipo de dados que será armazenado.

**NoSQL:** A ideia não é substituir o BD relacional, mas poder contar com capacidades adicionais que os relacionais oferecem. NoSQL surgiu quando começamos a contar com cenários que exigiam mais, principalmente em escalabilidade horizontal, quando começamos a tratar grandes volumes de dados e, principalmente, informações não estruturadas e tipos de dados não convencionais.

Independentemente do contexto, é preciso conhecer para escolher com segurança o BD que será usado em um projeto.

### • O NoSQL não foi criado para substituir o SQL?

BD relacionais conseguem garantir mais integridade de dados.

NoSQL não foi criado para substituir BDs relacionais. NoSql veio para atender ao que não conseguimos fazer com BDs relacionais, como forma de acrescentar mais ferramentas. Eles são e devem ser vistos como complementares.

Fatores importantes para sua utilização: dados desestruturados (schema não rígido), escalabilidade horizontal, alto volume de dados, consultas a estes dados (os dados já podem ser armazenados de modo a atender as consultas necessárias).

### • Como se consulta um dado armazenado no NoSQL, já que ele não tem compromisso com uma estrutura previamente conhecida?

Pode parecer ótimo pensar que trabalhar com um schema flexível, que isso é uma garantia de que o schema não encontrará dificuldades para armazenar dados, que não vai quebrar, mas como consultar dados em um schema onde um certo atributo pode não estar presente nos dados?

- Não ter um schema rígido não significa não precisar tomar cuidados básicos com o armazenamento.

- Ter um grande repositório de dados, mas não ter possiblidade de encontrar um dado no meio deles, não é vantajoso.

- Mesmo em um schema flexível, é preciso definir as chaves dos dados e as formas como será preciso consultar os dados no futuro.

- Do lado da aplicação, ela tem que estar preparada para trabalhar com a falta de algum atributo da informação.

- É essencial fazer uma modelagem de dados, pensando nas chaves e demais atributos que devem constar na estrutura dos dados.

### • Conhecer um SGBD de cada tipo é suficiente para iniciar?

- Conhecer os tipos de BDs é importante e fundamental.
- BDs relacionais, embora possuam particularidades, basicamente possuem o mesmo propósito.
- BDs NoSql possuem estruturas diferentes para finalidades específicas (chave-valor, grafos, etc).
- Primeiro deve-se conhecer a essência e o propósito de cada arquitetura.
- É muito positivo entender primeiro o contexto (a necessidade) e depois partir para escolha da tecnologia e aprofundamento técnico que esta exige.

### • A flexibilidade do NoSQL frente ao SQL

No início NoSQL trabalhava com consistência eventual, atualmente já existem BDs NoSQL que implementam algumas das propriedades ACID.

8base: fundada em 2017 (https://www.8base.com), esta é uma Plataforma de Aceleração de Desenvolvedor que capacita desenvolvedores e empresas de front-end a criar e executar facilmente aplicativos de software poderosos rapidamente usando o GraphQL.

GCP (google cloud platform): plataforma que reúne vários serviços de computação em nuvem que são usados para criar inúmeras soluções empresariais baseadas em Big Data, Inteligência Artificial, armazenamento em nuvem, entre outros.

### • Sobre DataLake, Data Warehouses e Databricks

**DataLake:** um repositório utilizado para armazenar todos os dados estruturados e não estruturados. Ao armazená-los de forma não estruturada pode-se realizar diferentes tipos de análise, incluindo processamento de big data, análise em tempo real e machine learning, a fim de adquirir melhores decisões.

**Data Warehouses:** armazena dados de forma mais estruturada de acordo com um objetivo pré-definido pelo time de dados.

**Databricks:** uma plataforma de análise baseada no Apache Spark. Projetado com os fundadores do Apache Spark, com o Databricks temos fluxos de trabalho simplificados e um workspace interativo que permite a colaboração entre os cientistas de dados, os engenheiros de dados e os analistas de negócios.

### • O tipo de banco de dados influencia na complexidade de ingestão, transformação e processamento dos dados?

É preciso pensar de início qual é a arquitetura que de fato será usada no BD: quais são as formas de consultas, quais são as chaves, quais índices devem ser previstos,...

Uma estratégia de arquitetura ruim do BD e de como os dados serão armazenados pode dificultar tanto o armazenamento quanto processos futuros de consulta.

### • Engenheiro e Cientista de dados são perfis complementares

**Engenheiro:** está mais ligado à preparação da informação: deve ter conhecimento técnico suficiente para coletar, armazenar de forma correta e deixar disponível para o restante da equipe de forma lógica e compreensível.

**Cientista:** é um dos “consumidores” da informação armazenada. Utiliza as informações disponibilizadas pelos engenheiros para gerar insights para o negócio (modelos preditivos, etc).

### • Dicas para quem quer ser Engenheiro de dados?
- Entender o que são dados em sua essência, como eles são captados e de que forma podem ser manipulados.
- Ferramentas são meios para se atingir objetivos.
- Ter amplo conhecimento do ecossistema de dados.
- Olhar crítico para saber aplicar tecnologias na solução de problemas.