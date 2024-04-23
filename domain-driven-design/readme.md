/\*
É uma forma de desenvolver software com foco no coração da aplicação(domínio), tendo o objetivo de entender as suas
regras, processos e complexidade, separando assim de outros pontos complexos que normalmente são adicionados durante
o desenvolvimento.
Grandes projetos falham por não ter modelagem, falta de clareza
DDD, deve ser aplicado em grandes projetos, pois em pequenos projetos não compensa o trabalho já que o core é pequeno
Não há como não utilizar técnicas avançadas em projetos de alta complexidade
Grande parte da complexidade de software não vem da tecnologia escolhida, mas sim da comunicação, separação de contextos
entendimento do negócio por diversos ângulos.
DDD, ajuda a:
Dar mais clareza ao que deve ser desenvolvido
Entender com profundidade os domínios e subdomínios da apliação
Ter uma linguagem universal entre todos os envolvidos no software
Criar o design estratégico utilizando Bounded Contexts
Clareza do que é complexidade técnica e complexidade do negócio

    Domínios e subdomínio, toda aplicação vai ter o seu domínio core e também seus subdomínios que fazem as ligações
    porém pode ser substituíveis mais facilmente

    Problemas = visão geral do domínio e suas complexidades, vai quebrar em subdomínios e com isso uma melhor análise do
    domínio possibilitando a criação de contextos limitados para cada subdomínio em específico
    Contexto é rei, se tiver a mesma palavra com significados diferentes você está em contexto diferentes

    Contexto conversam entre entidades, mas com perspectivas diferentes

    Modelagem é necessário ter uma visão geral de como as coisas estão se encaixando, para delimitar os contextos e definir
    como vão se conversar e se organizar.

    Possibilidade de criação de um time para cada contexto vai separar e deixar um grupo mais interado com o contexto
    Um contexto pode se encadrar como um fornecedor e outro contexto como cliente
    Padrões:
    Partinership
    Shared Kernel
    Costumer-Supplier development
    Conformist
    Anticorruption-level
    Open host service
    Pushided language
    Separete ways
    Big Ball of mud

    github context mapping

\*/
