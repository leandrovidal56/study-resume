# DDD

**Domain Driven Design**

### Livros de referencia:

[Tackling Complexity in the Heart of Software](https://acesse.one/EricEvans)

[Implementando Domain-Driven-Design](https://l1nk.dev/VaughnVernon)

[Domain-Driven-Design-Distilled](https://l1nk.dev/DDD-Destilado)

É uma forma de desenvolver software com foco no coração da aplicação(domínio), tendo o objetivo de entender as suas regras, processos e complexidade, separando assim de outros pontos complexos que normalmente são adicionados durante o desenvolvimento.

Grandes projetos falham por não ter modelagem, falta de clareza.
DDD, deve ser aplicado em grandes projetos, pois em pequenos projetos não compensa o trabalho já que o core é pequeno.
Não há como não utilizar técnicas avançadas em projetos de alta complexidade
Grande parte da complexidade de software não vem da tecnologia escolhida, mas sim da comunicação, separação de contextos e entendimento do negócio por diversos ângulos.

### DDD, pode ajudar?

Dar mais clareza ao que deve ser desenvolvido.
Entender com profundidade os domínios e subdomínios da apliação.

    - Domain é algo que está ligado a função principal da idéia de desenvolvimento do software ou podemos dizer o coração do software.

    - Subdomínios, são partes do nosso sistema que juntos se combinam e agregam valor ao produto.

Ter uma linguagem universal entre todos os envolvidos no software, sejam eles clientes, negócio, desenvolvedores, usuários e etc...

Criar o design estratégico utilizando Bounded Contexts:

    Saber que temos domínio, diversos subdomínios e baseados neles criar uma estratégia de modelagem para criar contextos e quando tiver esses contextos que vamos ter uma visão de tudo o que temos que desenvolver, mas apenas isso não vai ser tudo, pois vamos precisar também de um design tático para conseguir mapear e agregar as entidades e objetos de valor da aplicação nos eventos que tudo vai ser gerado. Juntando o olhar estratégico e tático.

Clareza do que é complexidade técnica e complexidade do negócio, a maior parte da dificuldade vai ser da complexidade de negócio.

Domínios e subdomínio, toda aplicação vai ser dividida em domínios que vão ser as maiores partes e também os subdomínios que vão compor os domínios.

Dentro de cada domínio ele vai ser composto pelo seu core domain, onde vai ser o coração do negócio o diferencial competitivo da empresa.

Subdomínio de suporte vai apoiar o dia a dia a tudo funcionar, mesmo não sendo o carro chefe principal
Subdomínio genérico não possui muito diferencial competitivo para a empresa e pode ser facilmente substituido.

Problemas = visão geral do domínio e suas complexidades, vai quebrar em subdomínios e com isso uma melhor análise do domínio possibilitando a criação de contextos limitados para cada subdomínio em específico.

Contexto delimitado é uma divisão explicita dentro de um domínio e quando a linguagem começa a mudar é que claramente deve estar entrando em outro contexto.

Contexto é rei, se tiver a mesma palavra com significados diferentes você está em contexto diferentes, e semopre vai determinar qual área da empresa estamos trabalhando.
Ticket dentro de venda de ingresssos e Ticket dentro de suporte ao clinte, nesse caso podemos observar claramente que a mesma palavra com significados totalmente diferentes e por isso precisamos isolar em contextos separados para que não tenhamos problemas.

Contexto conversam entre entidades, mas com perspectivas diferentes.

Modelagem é necessário ter uma visão geral de como as coisas estão se encaixando, para delimitar os contextos e definir como vão se conversar e se organizar.

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

[Context mapping](https://github.com/ddd-crew/context-mapping?tab=readme-ov-file)
