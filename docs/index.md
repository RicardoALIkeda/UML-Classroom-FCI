<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>



- [Autores](#nome-alunos)
- [Descrição do projeto](#introdução-do-projeto)
- [Análise de requisitos funcionais e não-fucionais](#descrição-dos-requisitos)
- [Diagrama de casos de uso](#diagrama-de-comportamento-atores)
- [Descrição dos casos de uso](#descrição-das-funcões)
- [Diagrama de senquencia](#diagrama-de-ordem-interações)
- [Diagrama de classes](#diagrama-orientado-objetos)
- [Diagrama de componentes](#diagrama-estrutura-componente)
- [Decisões de arquitetura](#decisões-de-arquitetura)
- [Diagrama de implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores

* Ricardo Andre Lopes Ikeda: 32158378


# Descrição do projeto

  &nbsp;A Pizza-Express é uma cadeia de 40 lojas de fast-food com entrega domiciliar.<br/>
	&nbsp;Pizza-Express vem perdendo 30% de seu rendimento em vendas por um problema em suas entregas. O problema está relacionado ao seu concorrente que disponibiliza uma entrega de até 30 minutos, desde o começo do pedido e a entrega.<br/>
	&nbsp;Pizza-express, disponibiliza de uma entrega de até 1 hora. Atualmente utiliza computadores para armazenar as operações e as funções usuais do negócio, que não auxilia nas funções de processamento da entrega de seus pedidos.<br/>
	&nbsp;O gerente de sistemas de informação, Elonn Muske, é encarregado de desenvolver uma aplicação de software que identifica a localização das lojas mais próximas do cliente e o sistema para operá-lo.<br/>
	&nbsp;Com o patrocínio de Papa-Léguas Delivery, a equipe deve investigar uma opção de entrega de menos de 30 minutos. A ideia principal é montar lojas da Pizza-Express que não possuam nenhum espaço de varejo, por ser focado apenas na produção e entrega de pizzas. A loja deve ser localizada o mais próximo do cliente que receberá a ordem através de uma central, processa, e a entrega a ordem dentro de 10 ou 15 minutos da entrada do pedido.<br/>
	&nbsp;Projetos de desenvolvimento de software indicados:<br/>
		&nbsp; &nbsp;-Software de atendimento, que encontra a localização da fábrica de pizzas mais próxima do cliente e a entregue;<br/>
		&nbsp; &nbsp;-Software de controle das operações da fábrica.<br/>


# Análise de requisitos funcionais e não-funcionais
&nbsp; -Sistema de localização<br />
&nbsp; -Sistema de pedidos<br />
&nbsp; -Rastreamento de pedidos<br />
&nbsp; -Controle de produção<br />
&nbsp; -Sistema de entrega<br />

# Diagrama de casos de uso


![Screenshot_9](https://github.com/RicardoALIkeda/UML-Classroom-FCI/assets/89215809/9f46feb4-79ec-4c2a-9a94-8f25e690da32)



# Descrição dos casos de uso

| Identificador  | UC01|
| ------------- | ------------- |
| Nome| Realizar pedido |
| Atores  | Cliente  |
| Sumário  | O Cliente usa o sistema para fazer seu pedido  |
| Pré-condição  | O Cliente deve estar logado  |
| Pós-condição  | O pedido é realizado  |
| Pontos de Inclusão  |   |
| Pontos de Extesão  |   |

| Identificador  | UC02|
| ------------- | ------------- |
| Nome| Realizar Login |
| Atores  | Cliente |
| Sumário  | Permite com que o Cliente se credencie no sistema  |
| Pré-condição  | Ter um cadastro ativo |
| Pós-condição  | Login realizado |
| Pontos de Inclusão  |   |
| Pontos de Extesão  |   |

| Identificador  | UC03|
| ------------- | ------------- |
| Nome| Encontrar loja mais proxima |
| Atores  |   |
| Sumário  | O sistema procura a unidade da Pizza-express mais proxima do cliente |
| Pré-condição  | Pedido ativo |
| Pós-condição  | O pedido é encaminhado para area de processamento |
| Pontos de Inclusão  |   |
| Pontos de Extesão  |   |

| Identificador  | UC04|
| ------------- | ------------- |
| Nome| Processar pedido |
| Atores  | Funcionario |
| Sumário  | O Funcionario processa as informações do pedido |
| Pré-condição  | Pedido ativo e a localização do cliente  |
| Pós-condição  | Envia as informações do pedido para fabrica  |
| Pontos de Inclusão  |   |
| Pontos de Extesão  |   |

| Identificador  | UC05|
| ------------- | ------------- |
| Nome| Controlar operações da fabrica  |
| Atores  | Funcionario |
| Sumário  | O funcionario encaminha as informações do pedido para os fabricantes  |
| Pré-condição  | Receber informações do pedido  |
| Pós-condição  | O funcionario indica o que deve ser feito com o pedido  |
| Pontos de Inclusão  |   |
| Pontos de Extesão  |   |

| Identificador  | UC06|
| ------------- | ------------- |
| Nome| Produzir pedido |
| Atores  |   |
| Sumário  | O Pedido é produzido  |
| Pré-condição  | Informações sobre o pedido  |
| Pós-condição  | Repassa o pedido ao entregador |
| Pontos de Inclusão  |   |
| Pontos de Extesão  |   |

| Identificador  | UC07|
| ------------- | ------------- |
| Nome| Entregar pedido |
| Atores  | Entregador |
| Sumário  | O entregador entrega o pedido ao cliente |
| Pré-condição  | Informações sobre a entrega do pedido e obter o pedido |
| Pós-condição  |   |
| Pontos de Inclusão  |   |
| Pontos de Extesão  |   |



# Diagrama de sequencia
![Screenshot_10](https://github.com/RicardoALIkeda/UML-Classroom-FCI/assets/89215809/901407b2-5d9d-4fb6-a522-07c299242edf)


# Diagrama de classes

![Screenshot_13](https://github.com/RicardoALIkeda/UML-Classroom-FCI/assets/89215809/e30adf29-203f-421b-a914-88968babdf8e)


# Diagrama de Componentes
![Screenshot_14](https://github.com/RicardoALIkeda/UML-Classroom-FCI/assets/89215809/e7c9bedc-4159-497d-887d-2dc96e523773)


# Decisões de arquitetura
Componentes Principais:

    Entrada:
        Aplicativo/Web para Pedidos e Rastreamento.
        Software de Atendimento para localização da fábrica.

    Processamento:
        Sistema de PDV para processamento e encaminhamento de pedidos.
        Servidores Locais para gerenciar lógica de negócios e integração.

    Banco de Dados:
        Centralizado para armazenar cardápio, pedidos, clientes e localizações.

    Saída:
        Impressoras na Fábrica para pedidos.
        Rastreamento de Entrega para informações em tempo real.

    Rede e Conectividade:
        Roteadores e Switches para manter conectividade.
        Conexão à Internet para pedidos online e atualizações.

    Sistema de Pagamento:
        Terminais de Pagamento e Gateway Online.

    Entrega:
        Rastreadores GPS para localização em tempo real.
        Comunicação com Entregadores para atualizações.

Arquitetura em Camadas:

    Apresentação (Interface do Usuário):
        Frontend Web responsivo e intuitivo.

    Lógica de Aplicação:
        Serviços e Lógica de Negócios para gestão de pedidos e entregas.
        Controladores para comunicação eficiente.

    Dados:
        Banco de Dados centralizado para consistência.


# Diagrama de implantação

![Screenshot_15](https://github.com/RicardoALIkeda/UML-Classroom-FCI/assets/89215809/5ff55979-7641-42fb-85d4-08894fbf1fc6)


# Referências

*&lt;Lista de referências&gt;*
