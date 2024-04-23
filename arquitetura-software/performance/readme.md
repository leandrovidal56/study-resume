/*
    Perpectivas para arquitetar um software 
        Performance
            É o desenpenho que o software possui para completar um determinado workload 
            latência ou response time 
            Throughput
            Ter software performático é diferente de escalável 
             Diminuir a latência se está demorando segundos ou invés de milisegundos já está bem ruim 
             Distância de data center interfere na performance devido a necessidade de uso de rede
             Aumentar o Throughput, permintindo que possa lidar com mais requisições e com retorno mais rápido 
        
        Principais razões de baixa performance do sistema
            Processamento ineficiente 
            Recursos computacionais limitados
            Trabalhar de forma bloqueante
            Soluções
                Escalar capacidade computacional 
                Melhorar lógica do software para ser mais performático 
                Concorrência e paralelismo, fazer várias coisas ou mesmo tempo
                Banco de dados, está correto? está modelado, estruturado?
                Caching, pode ser mais utilizado para ser reutilizado e poupar processamento 
        
        Escala concorrência e paralelismo
            Escala vertical para aumentar a capacidade pode aumentar a capacidade computacional 
            Escala horizontal para aumentar a capacidade pode aumentar a capacidade de máquina, geralmente com o load balance
            Concorrência é lidar com muitas coisas ao mesmo tempo e paralelismo é fazer muitas coisas ao mesmo tempo
        
        Caching
            Cache na borda/edge computing não chega nem a bater no seu servidor principal 
            Dados estáticos 
            Páginas web
            Funções internas, evita o reprocessamento de algorítmos pesados 
            Objetos 
            Compartilhado x Exlusivo 
            Exclusivo = baixa latência, duplicidade, problemas com sessões 
            Compartilhado = maior latência devido a dados centralizados, porém não existe duplicação de dados, sessões compartilhadas
                banco de dados de forma externa 
        
        Caching vs Edge Computing 
            Edge computing fazer com que os dados estajam mais próximos sem precisar bater direto no servidor
            Cache mais próximo do usuário(localidade sem a necessidade de bater em um servidor no EUA)
            Normalmente arquivos estáticos(cloudFare)
            CDN(Content Delivery Network)
            CloudFare workers 
*/
