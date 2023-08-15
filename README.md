# Banco_dados_ecommerce_ifood_desafio_projeto

Este desafio tinha o objetivo de refinar um modelo de banco de dados proposto pela instrutora do Bootcamp Ciência de Dados DIO/Ifood,
porém eu entendo que mais do que armazenar e resgatar informações, o banco de dados deve ser prático e útil, por isso, eu optei por 
simplificar o modelo, fazendo o melhor possível nas condições propostas.

Por exemplo, incialmente eu tinha desenhado o banco de dados com outras 2 tabelas, a de entrega e a de pagamento, mas no momento de 
inserir os dados, eu percebi que não fazia sentido persistir informações  como 'entrega em andamento', pois este é um tipo de 
informação tratada no API e que não deve ser persistida. Da mesma forma, informações bancárias são sigilosas e também não devem ser
persistidas no banco de dados do ecommerce.
Outras situações com as quais me deparei foram a existência de valores distintos de taxa de serviço e entrega, conforme a opção da 
loja parceira e distância, informações que dependem do API para serem geradas, filtradas e persistidas.
Também a possibilidade de clientes de pessoa jurídica e de entregadores com veículo do tipo bicicleta, que não requer placa e
licenciamento... A minha opção nesses casos foi restringir a inserção de dados e prezar pela segurança - não quero persistir um cpf 
com 13 dígitos!
Enfim, este projeto não visa ser um modelo completo e exaustivo de banco de dados, mas, antes, ser um exemplo de ferramente concisa, 
segura e prática a partir da qual coletar informações pertinentes para orientar tomada de decisão.

Em relação às queries elaboradas, também optei pela utilidade das mesmas e não por apresentar todo o repertório aprendido.
Eu dividi as queries em 4 partes, considerando os tipos de perfil: a 1a para traçar o perfil do consumidor, a 2a das lojas parceiras, 
a 3a dos produtos e a 4a dos entregadores parceiros.
Dessa forma, a empresa consegue entender claramente quem compõe seu quadro de clientes e parceiros, quais seus pontos fortes e 
fracos e onde concentrar esforços e recursos para melhorar ainda mais seus resultados.
Também evitei expor dados pessoais e sigilosos nas queries, por motivos de segurança das informações.
