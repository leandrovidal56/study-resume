/*
    Rest, Representational state of transfer 
        simplicidade sem guardar estado e possibilidade de cacheamento
        Níveis de maturidade 
            0 quando não tem nenhuma padrozinação
            1 Utilização de resources substantivo do que estiver trabalhando
            2 Verbos com representatividade e utilização correta como put, post, delete e get cada um na sua função específica
            3 HATEOAS, (Hypermedia as the Engine of Application State), sempre vai responder e trazer o que mais vai poder
                realizar com outras chamadas relacionadas, exemplo: get/aluno ai vai trazer 
                links:{ 
                    get/aluno/note
                    get/aluno/frequency
                    get/aluno/subject
                }
        Method e Content Negotiation
            Utilizar uri's únicas para serviços e itens expostos por esse serviço
            Utilizar todos os verbos HTTP para realizar operações em seus recursos, incluindo o caching 
            Mostrar links relacionais para os recursos exemplificando o que pode ser feito 
        Options, permite informar quais métodos vão ser permitidos ou não em determinado recurso
        
        ContentTypeNegociate, servidor irá verificar se vai conseguir suportar a informação enviada
        Accept whitelist, tipo de conteúdo que eu quero de retorno
        ContentType whitelist, tipo de conteúdo que eu vou mandar para a api processar 
    
    GraphQl
        Enviada de um formato onde o servidor entende o que exatamente o que você quer para ser retornado
        Mutation, para alterar ou criar dados
        Precisa injetar a depedência interna da aplicação para o graphql conseguir acessar
    Grpc
        Framework desenvolvido pelo Google com objetivo de facititar o processo de comunicação entre sistemas de uma 
        forma extremamente rápida, leve independentemente da linguagem. 
        ideal para microserviços
        Mobile, Browsers e Back-end
        Geração das bibliotecas de forma automática
        Streaming bidirecional utilizando HTTP/2
        Server streaming pode retornar pedaços em responses pequenas 
        Client streaming pode mandar em pedaços pequenos para o server
        Trabahar de forma bidirecional

    Service Discovery e consul 
        Descobre máquinas disponíveis para acesso
        Segmentação de máquinas para garantir a segurança
        Resoluções via DNS
        Health check ativo
        Como saber se tenho permissão para acessar
        
    Hashicorp Consul
        Service Discovery
        Service Segmentation
        Load balance na borda
        Key/value configuration
    Service Registry, vai centralizar todos os serviços e ter o controle qual está saudável para uso
    Multi cloud
    Agent, processo que fica sendo executado em todos os nós do cluster. Pode estar sendo executado em Client Mode ou
        Server Mode
    Client, registra os serviços localmente, Health Check, encaminha as informações e configurações dos serviços para o Server
    Server, mantém o estado do cluster, registra os serviços, Membership(quem é client e quem é Server), retorno de 
        queries(Dns ou Api), troca de informações entre datacenters e etc... e também é totalmente stateless, retorna os
        resultados dos serviços dele
    DevMode
        Roda como servidor, não escala e registra tudo em memória
*/
