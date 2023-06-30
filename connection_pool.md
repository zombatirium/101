Na engenharia de software, 
um pool de conexões é um cache de conexões de banco de dados 
mantido para que as conexões possam ser reutilizadas 
quando solicitações futuras ao banco de dados forem necessárias. 

Os conjuntos de conexões 
são usados para aprimorar o desempenho da execução de comandos em um banco de dados. 

Abrir e manter uma conexão de banco de dados para cada usuário, 
especialmente solicitações feitas 
a um site dinâmico 
baseado em banco de dados, 
é caro e desperdiça recursos. 

No pool de conexões, 
depois que uma conexão é criada, 
ela é colocada no pool e é usada novamente 
para que uma nova conexão 
não precise ser estabelecida. 

Se todas as conexões estiverem sendo usadas, 
uma nova conexão será feita e adicionada ao pool. 

O pool de conexões também reduz o tempo que um usuário 
deve esperar para estabelecer uma conexão com o banco de dados.
