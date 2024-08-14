# Sistema de PDV - Restaurantto App

## Introdução

### Motivação

O Restauranto nasceu da necessidade de automatizar processos em restaurantes e lanchonetes. Este sistema de gerenciamento foi projetado especificamente para atender às demandas desse setor, aumentando a produtividade de todos os envolvidos no restaurante: desde o chefe de cozinha, que cria e disponibiliza as receitas no cardápio, até o cliente, que pode acessar o menu digital e fazer pedidos diretamente pelo sistema.

### Contexto Atual

Vivemos em um momento em que a automação de tarefas é essencial em diversos setores, visando maximizar lucros e produtividade, ao mesmo tempo em que se evitam custos desnecessários. No setor alimentício, essa tendência é igualmente relevante – restaurantes e lanchonetes precisam garantir uma experiência satisfatória para seus clientes através de serviços automatizados, como:

1. Cardápio Digital

2. Controle de Caixa

3. Sistema de delivery

4. Pagamento facilitado

5. Controle de estoque

## Perfis de Usuário

### Persona 1 - Cliente

Os clientes são um dos pilares do sistema, com acesso ao cardápio digital do restaurante. Eles têm duas funções principais no sistema:

1. Escolha de itens do cardápio: Os clientes podem acessar o cardápio, informar ao garçom os itens desejados e as quantidades. Nesta modalidade, os clientes apenas visualizam os itens do cardápio.

2. Realização de pedidos via delivery: Os clientes podem fazer pedidos por meio de plataformas como iFood, e o sistema reconhece automaticamente esses pedidos através de uma integração.

### Persona 2 - Garçom

Os garçons atuam como intermediários entre os clientes e a cozinha, sendo responsáveis pelo lançamento dos pedidos no sistema, com detalhes sobre quantidade e itens solicitados, quando os clientes optarem por ir ao restaurante.

### Persona 3 - Chefe de Cozinha

Os chefes de cozinha gerenciam os pedidos realizados, podendo adicionar, listar, atualizar e deletar pedidos conforme sua prioridade (por exemplo, por ordem de chegada).

### Persona 4 - Gerente de restaurante

Os gerentes têm acesso a todas as funcionalidades do sistema, além de uma área administrativa exclusiva, onde podem ver informações como faturamento, número de vendas, entre outras.

## Requisitos Funcionais e Não-Funcionais do projeto

### Requisitos funcionais

Para o funcionamento do sistema de forma a satisfazer todas as *Personas* descritas, temos os seguintes requisitos:

1. Gerenciamento de Pedidos:
    * O sistema deve permitir que os chefes de cozinha recebam e visualizem os pedidos enviados pelo garçom em tempo real.
    * O sistema deve permitir que os garçons criem pedidos **personalizados**, isto é, os itens do cardápio são personalizáveis.
    * O sistema deve permitir que os pedidos feitos via plataformas de aplicativo, como Ifood e Rappi, sejam visualizados pelos chefes de cozinha.
    * O sistema deve permitir a marcação dos pedidos em **status**, estes, como: "em preparação", "em espera" e "pronto para servir" (ou "em entrega").

2. Priorização de Pedidos:
    * O sistema deve permitir que os pedidos sejam priorizados de acordo com o **tempo de solicitação** ou **tipo de prato**.

3. Atualização de Status do Pedido:
    * O sistema deve permitir que o chef atualize o status de um pedido em cada etapa da preparação (ex: “em preparação”, “preparado”, “servido”/"entregue").

4. Notificações e Alertas:
    * O sistema deve enviar notificações para a equipe de cozinha quando um pedido novo é recebido ou quando há um pedido urgente.

5. Relatórios de Produção:
    * O sistema deve gerar relatórios diários de produção, listando o número de pratos preparados, tempo médio de preparo e desperdício de ingredientes.

6. Gerenciamento de Ingredientes:
    * O sistema deve permitir o controle de estoque de ingredientes, alertando a equipe quando o nível de um item estiver baixo.
    * O sistema deve alertar aos usuários quando um ingrediente estiver em falta, tornando o status do pedido realizado

7. Interface de Usuário para Chefes e Cozinheiros:
    * O sistema deve oferecer uma interface amigável para que os chefs e cozinheiros possam acessar rapidamente as informações necessárias para a preparação dos pratos.

8. Histórico de Pedidos:
    * O sistema deve manter um histórico dos pedidos feitos, permitindo a consulta e análise posterior.

9. Integração com plataformas externas de delivery
    * O sistema deve integrar-se a plataformas para receber automaticamente os pedidos feitos pelos clientes via plataformas externas de delivery.

### Requisitos Não-Funcionais

1. Desempenho:
    * O sistema deve processar e exibir os novos pedidos na interface da cozinha em no máximo 2 segundos após o recebimento.

2. Escalabilidade:
    * O sistema deve suportar o aumento do número de pedidos sem degradação de desempenho, podendo lidar com picos de até 200 pedidos por hora.

3. Confiabilidade:
    * O sistema deve ter uma disponibilidade de 99,9%, garantindo operação contínua durante o horário de funcionamento do restaurante.

4. Segurança:
    * O sistema deve garantir que apenas usuários autenticados possam acessar e alterar as informações dos pedidos e do estoque.

5. Usabilidade:
    * A interface do sistema deve ser intuitiva e fácil de usar para cozinheiros com pouca experiência em tecnologia, permitindo a realização das tarefas com um mínimo de treinamento.

6. Manutenibilidade:
    * O sistema deve ser fácil de manter, com código modular e bem documentado, para facilitar futuras atualizações e correções.

7. Portabilidade:
    * O sistema deve ser compatível com diferentes tipos de dispositivos, incluindo tablets e computadores desktop utilizados na cozinha.

8. Eficiência Energética:
    * O sistema deve ser otimizado para consumo mínimo de energia, especialmente se for utilizado em dispositivos móveis.

9. Tecnologias Aplicadas:
    * A principio utilizaremos tecnologias e frameworks de desenvolvimento, tais quais: Angular (Front-end), NestJS (Back-end), PostgreSQL (Banco de Dados) e Kotlin (mobile).

10. Cenário de Execução:
    * O PDV será criado para ser executado em desktop e mobile. Utilizaremos de ferramentas de experiência de usuário para realizar o projeto da melhor e mais eficaz maneira.
