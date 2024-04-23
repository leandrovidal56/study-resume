/*
    Escalabilidade é a capacidade de sistemas suportarem o aumento ou redução dos 
    workloads incrementando ou reduzindo em menor ou igual proposção
    Enquanto performance busca diminuir a latência a aumentar troughput a 
    escalabilidade busca termos a possiblidade de aumentar ou diminuir o 
    troughput adicionando ou removendo a capacidade computacional.

    Escalando aplicações
        qualquer momento deve ser possível aumentar e diminuir a quantidade de máquinas
        Disco efêmero, tudo o que salvar em disco pode ser apagado a hora que precisar
            o disco deve ser usado para arquivos descartáveis 
        Servidor de aplicação vs Servidor de assets, é bom separar para poder escalar o específico para cada uso
        Cache centralizado, em servidor externo onde todas às máquinas irão buscar
        Sessões centralizadas 
        Upload e gravação de arquivos separados da máquina
    
    Escalar banco de dados
        Aumento de recursos computacionais, mas tem limite
        Distribuir responsabilidades exemplo um banco para escrita e outro para leitura se for muito grande pode ter várias
        máquinas de leitura ou mudar o formato do banco de dados ou até fazer partições
        Serveless, quando não se preocupar com servidores e deixa os cloud provaders escolherem essa parte
        Trabalhar com índices de forma correta 
        Usar APM(Application performance monitor) nas querys
        Explain para mostrar passo a passo das querys no banco 
        Usar CQRS(Command Query Responsibility Segregation), separar commando e query
    
    Proxy Reverso
        Servidor que fica na frente dos servidores web e encaminha as solicitações do cliente(por exemplo, nagevador web)
        para servidores web.
*/
