# Oficina
Este é um esquema conceitual para um sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica. O objetivo é registrar e gerenciar as ordens de serviço geradas para veículos de clientes, envolvendo equipes de mecânicos, serviços a serem executados e peças necessárias.

Entidades:

Cliente: Armazena informações sobre os clientes, como id, nome, endereço e telefone.
Veiculo: Registra os veículos dos clientes, com id, placa, modelo e ano.
Equipe: Representa as equipes de mecânicos que trabalham na oficina, com id e nome.
Mecanico: Armazena dados dos mecânicos, como id, nome, endereço e especialidade.
Ordem_de_Servico: Registra as ordens de serviço geradas, com id, data de emissão, data de entrega, valor total e status.
Servico: Armazena os serviços que podem ser executados na oficina, com id, descrição e valor da mão de obra.
Peca: Registra as peças que podem ser utilizadas nos serviços, com id, descrição e valor.

Relacionamentos:

Pertence: Relaciona clientes e veículos, indicando quais veículos pertencem a cada cliente.
Compoe: Relaciona equipes e mecânicos, indicando quais mecânicos compõem cada equipe.
Gera: Relaciona veículos e ordens de serviço, indicando quais ordens de serviço foram geradas para cada veículo.
Requisita: Relaciona ordens de serviço e serviços, indicando quais serviços foram requisitados em cada ordem de serviço.
Utiliza: Relaciona ordens de serviço e peças, indicando quais peças foram utilizadas em cada ordem de serviço, bem como a quantidade.
