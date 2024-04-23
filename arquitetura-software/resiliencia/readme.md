/*
    Resiliência é um conjunto de estratégias adotadas inicialmente para adaptação
    de um sistema quando uma falha ocorre.
    Ter estratégias de resiliência nos possibilita minimizar os riscos de de dados
    e transações importantes para o negócio.

    Quais estratégias de resiliência
        Proteger e ser protegido, contribuir para todo o ecosistema está saudável e não apenas um sistema só ser atendido
        Um sistema lento muitas vezes é pior que um sistema fora do ar

    Health check
        Precisa monitorar a saúde do sistema, com mecanismo que periodicamente mostre a situação do sistema
        Um sistema que não está saudável pode se recupar se o tráfego parar de ser redirecionado para ele.

    Rate limiting 
        Protege o sistema no que ele foi baseado para suportar, para isso é aconselhável a ser feito teste de estresse
        Preferência programada por tipo de cliente 
    
    Circuit Braker 
        Proteje o sistema fazendo com que as requisições que sejam redirecionadas para ele sejam negadas ex:500
            Circuito fechado, quando as requisições chegam normalmente 
            Circuito aberto, quando o circuito não está aguento e todas as chamadas retornam erro tipo 500
            Circuito meio aberto, permitida quantidade limitada para verificação se o sistema tem condições de voltar 
            normalmente
    
    Api Gateway
        Centraliza o recebimento de todas as requisições e aplicar regras para seguir ou barrar as requisições
    
    Service Mesh
        Controlar o tráfego de rede
        Circuit braker, timeout, retry tudo de forma automática

    Comunicação assincrona 
        fila é sempre comum em nossa vida cotidiana exemplo mercados, bancos e etc. Quem quiser se comunicar comigo vai 
        entrar na fila para trabalhar de forma assincrona. 

    Garantias de entrega com Retry
        Garantir que a mensagem está chegando no destino final, muitas vezes o retry de forma linear não adianta muito,
            ex: bateu 10 requisições e todas foram rejeitadas se tentar as 10 novamente juntas depois de 2 segundos vai
            quebrar também, por isso é melhor usar técnicas de exponencial backoff, exemplo espero 2,4,8,16... segundos
            para fazer o retry, e também utilizar com Jittler para evitar tentativas simultâneas.
    
    Situações complexas
        o que acontece se o seu broker cair? 
*/
