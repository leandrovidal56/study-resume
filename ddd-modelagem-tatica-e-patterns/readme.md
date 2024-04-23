    DDD começa com o entendimento da complexidade do software, mapear o domínio, criar um linguagem universal, criar
    contexto, bunded context, seperar o espaço do problema e da solução, e quando tiver os elementos estratégicos
    definidos que vamos para a parte tática.

    Precisamos resignificar conceitos e entender realmente como funciona e o que é, e não ser apenas como o macaquinho
    do jato de água e fazer as coisas por impulso e sem entendimento.

    Elementos táticos
    Quando estamos falando de DDD precisamos olhar mais a fundo um bounded context.
    Precisamos ser capazes de modelarmos de forma mais assertiva os seus principais componentes, comportamento e
    individualidades e suas relações.

    Entities, é algo único capaz de ser alterado de forma contínua durante um período de tempo. possível entender a individualidade.
    Possui uma continuidade no seu ciclo de vida e pode ser distinguida independente dos atributos que são importantes
    para a aplicação do usuário. Poder ser uma pessoa, cidade, carro, transação bancária ou um ticket de loteria.

    Entidade = identidade

    Toda vez que criar uma entendidade devo pensar nos atributos, pois são eles que vão mapear e o que vai mudar e toda
    vez que pensar em motivo para mudança é sobre regra de negócio.

    Entidade sempre vai representar o estado correto e atual daquele elemento
    Entidade ela sempre vai se autovalidar

    Entidade é focada em negócio = entidade
    Entidade é focada em persistência = orm

    é melhor ter duas entidades, exemplo de separação

    Complexidade de negócio
    Domain
        -Entity
        - - Costumer.ts(regra de negócio)

    Complexidade acidental
    Infra(mundo externo)
        -Entity(model)
        - - Costumer.ts(get, set)

    Quando você se preocupa apenas com os atributos de um elemento de um model, classifique isso como Value Object.
    trate o Value Object como imutável

    precisamos modelar de forma mais expressiva

    Agregado, é um conjunto de objetos associados que tratamos como uma unidade para propósito de mudança de dados.
