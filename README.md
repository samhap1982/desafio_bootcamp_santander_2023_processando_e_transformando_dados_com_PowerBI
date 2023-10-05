# Processando e transformando dados com PowerBI #

Repositório relacionado a formação de Power BI Analyst

Diretrizes para transformação dos dados

1. Verifique os cabeçalhos e tipos de dados
- OK

2. Modifique os valores monetários para o tipo double preciso
- Tabela employee: coluna salary alterei tipo de dados de número decimal para número decimal fixo;

3. Verifique a existência dos nulos e analise a remoção
- Existe um NULL na linha 5 (James E Borg) na tabela employee pórem se trata de um gerente.

4. Os employees com nulos em Super_ssn podem ser os gerentes. Verifique se há algum colaborador sem gerente
- Nenhum colaborador está atrelado a nenhum gerente

5. Verifique se há algum departamento sem gerente
- Não há

6. Se houver departamento sem gerente, suponha que você possui os dados e preencha as lacunas
- Vide resposta acima

7. Verifique o número de horas dos projetos
- OK 

8. Separar colunas complexas
- Dividi a coluna adress em street, number, city, state 

9. Mesclar consultas employee e departament para criar uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee. Fique atento, essa informação influencia no tipo de junção
- OK

10. Neste processo elimine as colunas desnecessárias.
- OK

11. Realize a junção dos colaboradores e respectivos nomes dos gerentes . Isso pode ser feito com consulta SQL ou pela mescla de tabelas com Power BI. Caso utilize SQL, especifique no README a query utilizada no processo.
- Mescla feita por Power Query

12. Mescle as colunas de Nome e Sobrenome para ter apenas uma coluna definindo os nomes dos colaboradores
- OK 

13. Mescle os nomes de departamentos e localização. Isso fará que cada combinação departamento-local seja único. Isso irá auxiliar na criação do modelo estrela em um módulo futuro.
- OK

14. Explique por que, neste caso supracitado, podemos apenas utilizar o mesclar e não o atribuir.
- O mesclar funde colunas de duas tabelas, o atribuir trabalha de maneira diferente

15. Agrupe os dados a fim de saber quantos colaboradores existem por gerente
- Existem 6 funcionários atrelados ao gerente Franklin T Wong, 3 funcionários atrelados ao gerente Jennfier S Wallace, 1 funcionário atrelado ao gerente Jame E Borg

16. Elimine as colunas desnecessárias, que não serão usadas no relatório, de cada tabela
- OK
