# Oficina Mecanica

### Objetivo  - Desafio da Dio de criar um esquema conceitual de banco de dados  do zero para atender uma suposta Oficina mecânica.



##### Narrativa: 

###### Sistema de controle e gerenciamento de Ordens de Serviço. O sistema recebe OS inicial com entrada de cadastro do cliente e do veículo a ser examinado por equipe técnica (mecânico), que irá identificar o tipo de serviço como conserto ou revisão e gera orçamento inicial com valores de mão de obra e peças á serem usadas. OS inicial tem data de entrada e previsão de entrega dos serviços.

- Equipe mecânica da OS inicial é a mesma que executa os serviços orçados;
- Mão de Obra e peças tem preços tabelados;
- OS  recebe autorização do cliente antes de iniciar os serviços;



##### Refinamentos:

###### Alguns refinamentos e melhorias foram aplicadas no tabelamento de orçamentos e na finalização da OS:

- Criou-se relação Peças, para tabelar valores de peças em estoque e peças disponíveis para compra em lojas parceiras previamente autorizadas e cadastradas;
- OS_autorizada - libera ordem de compra de peças em lojas autorizadas (quando necessário) e inicio de serviços, após orçamento aprovado pelo cliente;
- Baixa de OS - Da baixa as OS_inicial e OS_autorizada vinculadas a ela, após conclusão dos serviços e pagamento do cliente.
- Método de pagamento - persiste informações de pagamento.

