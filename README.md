# desafio_engenharia_dados
Repositório para armazenar casos de uso voltados a engenharia de dados.


Caso de uso para ser explorado com o candidato para entrevista de engenharia de dados, que valida conhecimentos técnicos em engenharia de dados, infraestrutura cloud Azure e Google, monitoramento de linhagem de dados e data mesh:

1. **Definição do cenário do problema**: A Fintech precisa de uma solução que permita coletar, processar e analisar grandes volumes de dados de transações financeiras em tempo real, garantindo a segurança e a integridade dos dados. A solução deve ser capaz de monitorar a linhagem de dados e implementar uma data mesh para gerenciar a qualidade e a segurança dos dados.

2. **Descrição dos requisitos técnicos**: O candidato deve ser capaz de configurar e gerenciar a infraestrutura Cloud Azure e Google, implementar uma estratégia de monitoramento de linhagem de dados e desenvolver uma data mesh.

***Arquitetura Atual, que deve ser alterada: Atualmente a aplicação está hospedada na Cloud Azure, como banco de dados transacional o Cosmos DB. O Data Lake está centralizado no Google Cloud. Portanto, todas as visões de dados estão consumindo relatórios que são compartilhados pelos parceiros via um repositório SFTP. Há processo automatizado para coletar estes arquivos e armazená-los no Google Cloud Storage. Estes arquivos disponibilizados no Storage, são processados através de uma função do BigQuery e disponibilizam os dados mais atuais em suas respectivas tabelas, que possuem dashboard do PowerBI conectados para visualização.

*** Arquitetura Futura, que deve ser explorada e definida pelo candidato. Observação: O candidato deve avaliar necessidade de criação de componentes para a infraestrutura de dados, para automatizar a coleta dos dados nas sources de origem, para posteriormente armanzenar no Data Lake. Deve ser explorado a necessidade de criação de monitoramento, e organização no Data Lake e Data Mash.


3. **Estabelecer a estratégia de monitoramento**: O candidato deve configurar a coleta de métricas e logs de todos os recursos para monitorar sintomas/condições que sejam problemas, que indiquem impacto potencial ou real para a disponibilidade do serviço ou impacto dos consumidores do serviço/aplicativo. O candidato também deve propor quais medidas devem ser estruturadas dos serviços para acompanhar se estão cumprindo contratos de serviço medindo o utilitário do serviço ou aplicativo. Citar exemplos.

4. **Definir a estratégia de data mesh**: Com a arquitetura futura que o candidato propor, deve ser alimentado com a proposta da arquiteturafutura para monitoramento, identificar lacunas de monitoramento e modelar os aspectos financeiros, custos e fatores de suporte que dão suporte a uma análise de custo-benefício.

5. **Estabelecer a estratégia de governança**: O candidato deve ser capaz de estabelecer como pretende controlar seu investimento de monitoramento de nuvem. O candidato também deve ser capaz de definir quem terá que nível de acesso no Google Cloud para dar suporte à sua função e responsabilidade.

6. **Definir a estratégia de preparação**: O candidato deve ser capaz de formular um plano de preparação para ajudar sua equipe de IT a adotar novas habilidades, práticas e técnicas para o monitoramento de nuvem no Azure e Google.

7. **Definir a estratégia de monitoramento para modelos de implantação em nuvem**: O candidato deve ser capaz de propor modelo de monitoramento para as pipelines desenvolvidas  (ingestão e transformação).

** Atividade a ser desenvolvida:
O Candidato deve ser capaz de estrutura um Desing System (desenho) da arquitetura futura que está propondo. Contendo os componentes que devem ser desenvolvidos (ETL), monitoramentos e estratégia de organização do Data Mesh.