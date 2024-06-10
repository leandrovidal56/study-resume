# Características Arquiteturais 

### Operacionais: 
- Disponibilidade pensar o quanto de disponibilidade vai oferecer ao seu cliente.
- Recuperação de desastres, se der algum problema como atuar? 
- Performance: qual a performance esse sistema deve ter? 
- Backup: qual foi a última vez que testou o backup? 
- Confiabilidade e segurança: qual o nível de segurança e confiança quer que seu sistema estaja preparado?
- Robustez: está em uma estrutura que suporta ser transferido de região da nuvem facilmente? 
- Escalabilidade: preparar o sistema para escalar de forma rápida e fácil.

### Estruturais:
- Configuração fácil, precisa ser fácil subir todos os ambientes e também trocar qualquer serviço.
- Extensibilidade para ser extensível para adicionar novos módulos e serviços.
- Fácil instalação, falta de padronização para ambientes de sua aplicação e é aconselhável pode ter dependências complexas.
- Reuso de componentes: usar o máximo de componentes possíveis para problemas diferentes.
- Internacionalização: verificar a necessidade de compartilhar partes do software.
- Fácil manutenção: executar rápido a manutenção.
- Portabilidade: é fácil mudar o banco de dados hoje?.
- Fácil suporte: deixar o mais fácil possível o suporte para resolver problemas.

### Cross-Cutting
- Acessibilidade: deixar o mais acessível possível a aplicação.
- Retenção e recuperação de dados: quais dados precisa utilizar com frequencia, separar dados para os não utilizados com frequência deixar em serviço mais barato.
- Autenticação e Autorização: como o seu sistema vai trabalhar a comunição entre serviços? 
- Legal: seguir normas do país.
- Privacidade: miticar os riscos de vazamento de dados.
- Segurança: sempre precisa estar de ponta a ponta.
- Usabilidade: tem documentação?, tem padrão?

Performance

Perfomance, Escalabilidade, Resiliência 
Performance nem sempre está ligada a escalabilidade 
	Diminuir latência (se demorar mais de segundos está ficando lento)
	Aumentar o throughpu (aumento de requisições simultâneas)
	Processamento ineficiente 
	Recurso computacionais limitados 
	Trabalhar de forma bloqueante 
