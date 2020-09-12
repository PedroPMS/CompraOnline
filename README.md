# TRABALHO 01:  CompraOnline
Trabalho desenvolvido durante a disciplina de BD1

# Sumário

### 1. COMPONENTES<br>
Integrantes do grupo<br>
Amanda Ferreira de Souza: amandas9764@gmail.com<br>
Ana Elisa Paim Dias Rezende: anaelisa0935@gmail.com<br>
Pedro Paulo Mauro e Silva: p.paulo0512@gmail.com<br>

### 2.INTRODUÇÃO E MOTIVAÇÃO<br>
Este documento contém a especificação do projeto do banco de dados <nome do projeto> 
<br>e motivação da escolha realizada. <br>

> O sistema "CompraOnline" visa ajudar pessoas a realizarem suas compras, evitando que elas saiam de casa, mantendo-as isoladas em meio à pandemia. Sabendo-se dos desafios para sair de casa e não se contaminar, e visando a proteção e comodidade dos clientes, ficamos motivados com o desenvolvimento deste sistema. O sistema em questão tem como objetivo tornar possível a compra de roupas e acessórios online. Para realizar suas operações adequadamente, o sistema armazena informações relativas ao cliente, além de também armazenar dados sobre os produtos. O sistema deverá gerar um compra que por sua vez atenderá os anseios dos clientes em questão. O objetivo inicial da empresa é oferecer produtos de vestuário ou acessórios para seus usuários de forma virtual, com objetivo de evitar aglomerações em tempos de pandemia.

 
### 3.MINI-MUNDO<br>

Descrever o mini-mundo! (Não deve ser maior do que 30 linhas, se necessário resumir para justar) <br>
Entrevista com o usuário e identificação dos requisitos.(quando for o caso de sistemas com cliente  real)<br>
Descrição textual das regras de negócio definidas como um  subconjunto do mundo real 
cujos elementos são propriedades que desejamos incluir, processar, armazenar, 
gerenciar, atualizar, e que descrevem a proposta/solução a ser desenvolvida.

> O sistema "CompraOnline" tem como objetivo oferecer opção para clientes fazerem compra de roupas e acessórios online. Para realizar as vendas, é necessário que o sistema armazene diversas informações. Para um usuário realizar compras no sistema, é necessário que ele faça uma conta, onde será armazenado seu nome, e-mail, senha, telefone, cpf e endereço. A compra é realizado pelo usuário e nele é contido a data que a compra foi realizada, preço total da compra. A compra contem os produtos que são identificados pelo seu nome, seu preço e quantidade escolhida pelo cliente. Uma compra pode ter um ou vários produtos. O usuário pode ter uma ou várias compras. Assim como cada compra pode ter um ou vários produtos.


### 4.PROTOTIPAÇÃO, PERGUNTAS A SEREM RESPONDIDAS E TABELA DE DADOS<br>
#### 4.1 RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
Neste ponto a codificação não e necessária, somente as ideias de telas devem ser criadas, o princípio aqui é pensar na criação da interface para identificar possíveis informações a serem armazenadas ou descartadas <br>

Sugestão: https://balsamiq.com/products/mockups/<br>

![Alt text](https://github.com/PedroPMS/CompraOnline/blob/master/images/tela_compraonline.PNG?raw=true "Balsamiq") 
![Arquivo PDF do Protótipo Balsamiq feito para Sistema CompraOnline](https://github.com/PedroPMS/CompraOnline/blob/master/arquivos/CompraOnline.pdf?raw=true "CompraOnline")
#### 4.2 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
     
    a) O sistema proposto fornece quais tipos de produtos?
    b) Qual o relatório pode ser obtido por meio desse Sistema?

> O Sistema CompraOnline fornece os seguintes produtos:

* Vestuário
* Acessórios 

> O sistema precisa inicialmente dos seguintes relatórios:

* Relatorio que mostre o nome de todos os clientes, sua identificação, produto comprado, seu preço, quantidade e o total da compra. Os resultados devem ser apresentados ordenados por produto.
* Relatório relativo aos produtos e compras. O resultado deverá mostrar qual o produto mais vendido do mês.
* Relatório que mostre as informação relacionadas ao faturamento do mês. O resultado deverá apresentar o valor total de vendas no mês.

 
#### 4.3 TABELA DE DADOS DO SISTEMA:
    a) Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas/registros de dados.
    b) Esta tabela tem a intenção de simular um relatório com todos os dados que serão armazenados 
    
![Exemplo de Tabela de dados do Sitema CompraOnline](https://github.com/PedroPMS/CompraOnline/blob/master/arquivos/TabelaEmpresaCompraOnline.xlsx?raw=true "Tabela - CompraOnline")
    
    
### 5.MODELO CONCEITUAL<br>
    A) Utilizar a Notação adequada (Preferencialmente utilizar o BR Modelo 3)
    B) O mínimo de entidades do modelo conceitual pare este trabalho será igual a 3 e o Máximo 5.
        * informe quais são as 3 principais entidades do sistema em densenvolvimento<br>(se houverem mais de 3 entidades, pense na importância da entidade para o sistema)       
    C) Principais fluxos de informação/entidades do sistema (mínimo 3). <br>Dica: normalmente estes fluxos estão associados as tabelas que conterão maior quantidade de dados 
    D) Qualidade e Clareza
        Garantir que a semântica dos atributos seja clara no esquema (nomes coerentes com os dados).
        Criar o esquema de forma a garantir a redução de informação redundante, possibilidade de valores null, 
        e tuplas falsas (Aplicar os conceitos de normalização abordados).   
        
![Alt text](https://github.com/PedroPMS/CompraOnline/blob/master/images/_conceitual.PNG?raw=true "Modelo Conceitual")
    
    
        
    
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: Aline Prasser, Luara Hombre
    Nenhuma recomendação foi dada.
    
    [Grupo02]: Gabriel Nascimento, Luiza de Alencar, Rebeca Borlini
    Recomendações dadas: "No minimundo tem algumas informações a mais sobre a tabela "Produtos", pois fala que tem o atributo quantidade, e não aparece no mapa, somente no "compra", e no usuário também, como a parte do telefone e endereço, não foi mencionado no texto, então parecia que não precisava."
    
#### 5.2 Descrição dos dados 
    USUÁRIO: Tabela com dados do usuário do sistema
     Id_usuario: campo que armazena a identificação do usuário
     Nome: campo que armazena o nome do usuário do sistema
     Cpf: campo que armazena o número de Cadastro de Pessoa Física para cada cliente do sistema
     Email: campo que armazena o e-mail do cliente do sistema
     Senha: campo que armazena a senha do cliente do sistema
     Endereço (estado, município, tipo de logradouro, logradouro, numero, bairro, cep): campo que armazena informações do endereço do usuário do sistema
     
    Compra: Relacionamento entre Cliente e Produto
     Id_compra: campo que armazena a identificação da compra do usuário
     Data_compra: campo que armazena a data que foi feita a compra pelo usuário
     Quantidade: campo que armazena a quantidade de produto que o usuário comprou no sistema
     
    PRODUTO: Tabela que armazena informações sobre os produtos da loja
     Id_produto: campo que armazena a identificação de cada produto vendido pela loja
     Nome: campo que armazena o nome de cada produto vendido pela loja
     Preco: campo que armazena o preço de cada produto vendido pela loja
    
    TELEFONE: Tabela que armazena o número de telefone do usuário do sistema
     Id_telefone: campo que armazena a identificação do número de telefone do usuário
     Id_usuario: campo que armazena a identificação do usuário que possui o número
     Numero_telefone: campo que armazena a identificação o número de telefone do usuário
     


### 6	MODELO LÓGICO<br>
        a) inclusão do esquema lógico do banco de dados
        b) verificação de correspondencia com o modelo conceitual 
        (não serão aceitos modelos que não estejam em conformidade)
        
![Alt text](https://github.com/PedroPMS/CompraOnline/blob/master/images/logico.PNG?raw=true "Modelo Logico")


### 7	MODELO FÍSICO<br>
        --CRIAÇÃO TABELAS--

        CREATE TABLE PRODUTO(
         id_produto integer not null, 
         nome varchar(15), preco float, 
         primary key(id_produto));

        CREATE TABLE TELEFONE(
         id_telefone integer not null, 
         id_usuario integer, 
         numero_telefone bigint, 
         primary key (id_telefone));

        CREATE TABLE USUARIO(
         id_usuario integer not null, 
         nome varchar(80), 
         cpf bigint, 
         email varchar(100), 
         senha varchar(15), 
         estado varchar(2), 
         municipio varchar(50),
         tipo_logradouro varchar(10), 
         logradouro varchar(50), 
         numero integer, 
         bairro varchar(30), 
         cep integer, 
         primary key(id_usuario));

        CREATE TABLE COMPRA(
         id_compra integer not null, 
         id_produto integer, 
         id_usuario integer, 
         data_compra date, 
         quantidade integer, 
         primary key(id_compra));
        
        --INCLUSÃO DE CHAVES ESTRANGEIRAS--

        ALTER TABLE TELEFONE ALTER COLUMN numero_telefone TYPE bigint
        ALTER TABLE USUARIO ALTER COLUMN cpf TYPE bigint

        ALTER TABLE TELEFONE
        ADD CONSTRAINT fk_USUARIO_telefone FOREIGN KEY (id_usuario) REFERENCES USUARIO(id_usuario) MATCH FULL ON UPDATE CASCADE ON Delete CASCADE;

        ALTER TABLE COMPRA
        ADD CONSTRAINT fk_USUARIO_id_usuario FOREIGN KEY (id_usuario) REFERENCES USUARIO(id_usuario) MATCH FULL ON UPDATE CASCADE ON Delete CASCADE;

        ALTER TABLE COMPRA
        ADD CONSTRAINT fk_USUARIO_id_produto FOREIGN KEY (id_produto) REFERENCES PRODUTO(id_produto) MATCH FULL ON UPDATE CASCADE ON Delete CASCADE;
        
       
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
        --DROP--
        DROP TABLE PRODUTO CASCADE;

        DROP TABLE TELEFONE CASCADE;

        DROP TABLE USUARIO CASCADE;

        DROP TABLE COMPRA CASCADE;

        --CRIAÇÃO TABELAS--

        CREATE TABLE PRODUTO(
         id_produto integer not null, 
         nome varchar(15), preco float, 
         primary key(id_produto));

        CREATE TABLE TELEFONE(
         id_telefone integer not null, 
         id_usuario integer, 
         numero_telefone bigint, 
         primary key (id_telefone));

        CREATE TABLE USUARIO(
         id_usuario integer not null, 
         nome varchar(80), 
         cpf bigint, 
         email varchar(100), 
         senha varchar(15), 
         estado varchar(2), 
         municipio varchar(50),
         tipo_logradouro varchar(10), 
         logradouro varchar(50), 
         numero integer, 
         bairro varchar(30), 
         cep integer, 
         primary key(id_usuario));

        CREATE TABLE COMPRA(
         id_compra integer not null, 
         id_produto integer, 
         id_usuario integer, 
         data_compra date, 
         quantidade integer, 
         primary key(id_compra));

        --INCLUSÃO DE CHAVES ESTRANGEIRAS--

        ALTER TABLE TELEFONE ALTER COLUMN numero_telefone TYPE bigint;

        ALTER TABLE USUARIO ALTER COLUMN cpf TYPE bigint;

        ALTER TABLE TELEFONE
        ADD CONSTRAINT fk_USUARIO_telefone FOREIGN KEY (id_usuario) 
        REFERENCES USUARIO(id_usuario) MATCH FULL ON UPDATE CASCADE ON Delete CASCADE;

        ALTER TABLE COMPRA
        ADD CONSTRAINT fk_USUARIO_id_usuario FOREIGN KEY (id_usuario) 
        REFERENCES USUARIO(id_usuario) MATCH FULL ON UPDATE CASCADE ON Delete CASCADE;

        ALTER TABLE COMPRA
        ADD CONSTRAINT fk_USUARIO_id_produto FOREIGN KEY (id_produto) 
        REFERENCES PRODUTO(id_produto) MATCH FULL ON UPDATE CASCADE ON Delete CASCADE;

        --INSERT--
        INSERT INTO PRODUTO(id_produto, nome, preco)
        VALUES (1, 'Macacão', 70),
               (2, 'Blusa', 25),
               (3, 'Calça', 300),
               (4, 'Meia', 5), 
               (5, 'Cinto', 25), 
               (6, 'Short', 70);

        INSERT INTO USUARIO(id_usuario, nome, cpf, email, senha, estado, municipio, tipo_logradouro, logradouro, numero, bairro, cep)
        VALUES (1, 'Amanda Ferreira', 12345,'amanda@gmail.com', '123@456', 'ES','Vila Velha', 'Rua', 'Olegario Mariano', 1338, 'Soteco', 29106240),
        (2, 'Ana Elisa Rezende', 12120, 'anaelisa@gmail.com', '123@456', 'ES','Serra','Rua','Carapebus', 105, 'Valparaiso', 29165813),
        (3, 'Pedro Paulo Silva', 99999, 'pedro@gmail.com', '123@456', 'ES', 'Vitória', 'Rua', 'Milton Ramalho Simões', 11, 'Jardim Camburi', 29090770),
        (4, 'Lucia Gonçalves',78789, 'lucia@gmail.com','123@456','ES','Vila Velha','Avenida', 'Carlos Lindemberg', 254, 'Araçás',29109600),
        (5, 'Julia Clarindo',81254, 'julia@gmail.com','123@456','ES','Cariacica','Rua', 'Emilio de Abreu', 254, 'Junqueira',29167841),
        (6, 'Paula Abreu',96547, 'paula@gmail.com','123@456','ES','Vila Velha','Avenida', 'Carlos Lindemberg', 256, 'Araçás',29109600),
        (7, 'Joao Junqueira',79996,'joao@gmail.com', '123@456', 'ES', 'Cariacica', 'Rua', 'Nova', 98, 'Orquidea', 29456123),
        (8, 'Viviane Reis',78452, 'viviane@gmail.com','123@456','ES','Vila Velha','Avenida', 'Carlos Lindemberg', 256, 'Araçás',29109600),
        (9, 'Thyago B', 54687, 'thyago@gmail.com', '123@456', 'ES','Serra','Rua','Carapebus', 105, 'Valparaiso', 29165813),
        (10, 'Fernando Henrique', 32659,'fernando@gmail.com', '123@456', 'ES','Vila Velha', 'Rua', 'Olegario Mariano', 1338, 'Soteco', 29106240);

        INSERT INTO TELEFONE(id_telefone, id_usuario, numero_telefone)
        VALUES (1, 1, 985470122), 
               (2, 2, 40028922), 
               (3,3, 08007777000), 
               (4,4,965441111), 
               (5,5,987445632), 
               (6,6,32180764), 
               (7,7,20021001), 
               (8,8, 30100259), 
               (9,9, 782145215), 
               (10,10, 54548181);

        INSERT INTO COMPRA(id_compra, id_produto, id_usuario, data_compra, quantidade)
        VALUES (1, 3, 1, '01-08-2020',1), 
               (2, 4, 2, '01-08-2020', 4), 
               (3, 6, 3, '01-08-2020',2), 
               (4, 5, 4, '01-08-2020',1),
               (5, 4, 5, '01-08-2020', 1), 
               (6, 3, 6, '01-08-2020', 2),
               (7, 4, 7, '08-28-2020', 1),
               (8, 6, 8, '08-28-2020', 2),
               (9, 1, 9, '08-28-2020' , 1),
               (10, 2, 10, '08-28-2020', 2);


### 9	TABELAS E PRINCIPAIS CONSULTAS<br>

#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>
    Select *
    From PRODUTO
![Alt text](https://github.com/PedroPMS/CompraOnline/blob/master/images/Select%20all%20From%20produto.PNG?raw=true "Produtos")
    </br>

    Select *
    From TELEFONE
![Alt text](https://github.com/PedroPMS/CompraOnline/blob/master/images/Select%20all%20From%20telefone.PNG?raw=true "Telefone")
    </br>
    
    Select *
    From USUARIO
![Alt text](https://github.com/PedroPMS/CompraOnline/blob/master/images/Select%20all%20From%20usuario.PNG?raw=true "Usuário")
    </br>

    Select *
    From COMPRA
 ![Alt text](https://github.com/PedroPMS/CompraOnline/blob/master/images/Select%20all%20From%20compra.PNG?raw=true "Compra")
    </br>


># Marco de Entrega 01: Do item 1 até o item 9.1<br>

#### 9.2	CONSULTAS DAS TABELAS COM FILTROS Where (Mínimo 4)<br>
    Select *
    From usuario
    Where municipio = 'Vitória'

    Select *
    From usuario
    Where tipo_logradouro = 'Rua'

    Select *
    From compra
    Where quantidade = 1

    Select *
    From telefone
    Where id_usuario = 1
    
#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    Select *
    From usuario
    Where bairro = 'Soteco' And tipo_logradouro = 'Rua'

    Select *
    From usuario
    Where municipio = 'Vitória' or municipio = 'Serra'

    Select *
    From produto
    Where preco = 25 or preco = 70

    Select *
    From compra
    Where data_compra = '2020-01-08' or quantidade = 2

    Select *
    From telefone
    Where numero_telefone Is Not Null


    Select *
    From produto
    Where preco > 60

    Select *
    From compra
    Where quantidade <= 3

    Select *
    From produto
    Where preco <= 30


    Select nome, estado as UF, municipio as cidade
    From usuario

    Select id_usuario as usuario, numero_telefone as telefone
    From telefone

    Select nome as produto, preco as valor
    From produto


#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    Select *
    From produto
    Where nome like '%a'

    Select *
    From usuario
    Where nome like 'A%a'

    Select *
    From usuario
    Where municipio ilike 'v%'

    Select *
    From usuario
    Where estado like 'E_'

    Select *
    From usuario
    Where tipo_logradouro ilike '___'

    
    Select *
    From compra
    Where data_compra = current_date

    Select data_compra, current_date as dia_atual, age(current_date,data_compra)
    From compra

    Select data_compra, date_part('days',data_compra)
    From compra

    Select isfinite(data_compra)
    From compra

    Select data_compra, extract('year' From data_compra) as ano_compra
    From compra

    Select concat(date_part('year',data_compra), ' qnt: ', quantidade)
    From compra

    Select *
    From compra
    Where data_compra = current_date



#### 9.5	INSTRUÇÕES APLICANDO ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>
    a) Criar minimo 3 de exclusão
    Delete From produto Where id_produto = 1
    Delete From compra Where id_compra = 9
    Delete From usuario Where id_usuario = 9
     
    b) Criar minimo 3 de atualização
    Update usuario
    Set nome = 'Joana Amaral', email = 'joana@gmail.com'
    Where id_usuario = 3

    Update produto
    Set preco = 10
    Where id_produto = 4

    Update telefone
    Set id_telefone = 9, numero_telefone = 989865654
    Where id_telefone = 10


#### 9.6	CONSULTAS COM Inner Join E Order BY (Mínimo 6)<br>
    a) Uma junção que envolva todas as tabelas possuindo no mínimo 2 registros no resultado
     Select usuario.nome, usuario.cpf, telefone.numero_telefone, produto.nome as nome_produto, compra.quantidade, compra.data_compra
     From usuario
     Inner Join telefone
     ON (telefone.id_usuario = usuario.id_usuario)
     Inner Join compra
     on (compra.id_usuario = usuario.id_usuario)
     Inner Join produto
     on (produto.id_produto = compra.id_produto)
     Order by compra.data_compra ASC
    
    b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
     Select usuario.cpf, produto.nome as nome_produto, compra.data_compra
     From usuario
     Inner Join compra
     on (compra.id_usuario = usuario.id_usuario)
     Inner Join produto
     on (produto.id_produto = compra.id_produto)
     Order by usuario.cpf

     Select usuario.nome, telefone.numero_telefone, compra.data_compra
     From usuario
     Inner Join telefone
     on (telefone.id_usuario = usuario.id_usuario)
     Inner Join compra
     on (compra.id_usuario = usuario.id_usuario)
     Order by compra.data_compra ASC

     Select usuario.cpf, produto.nome, compra.quantidade
     From usuario
     Inner Join compra
     on (compra.id_usuario = usuario.id_usuario)
     Inner Join produto
     on (produto.id_produto = compra.id_produto)
     Order by produto.nome

     Select usuario.nome, telefone.numero_telefone, usuario.email, usuario.estado, usuario.bairro
     From usuario
     Inner Join telefone
     on (telefone.id_usuario = usuario.id_usuario)
     Order by usuario.bairro

     Select usuario.cpf, usuario.municipio, usuario.tipo_logradouro, usuario.logradouro, usuario.bairro, compra.data_compra
     From usuario
     Inner Join compra
     on (compra.id_usuario = usuario.id_usuario)
     Order by usuario.municipio

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>
    a) Criar minimo 2 envolvendo algum tipo de junção
     Select nome as nome_produto, count(*)
     From produto
     Inner Join compra
     on (produto.id_produto = compra.id_produto)
     group by nome

     Select usuario.nome, produto.nome as nome_produto, MAX(preco)
     From produto
     Inner Join compra
     on (produto.id_produto = compra.id_produto)
     Inner Join usuario
     on (compra.id_usuario = usuario.id_usuario)
     group by usuario.nome, produto.nome

     select produto.nome, produto.preco, compra.data_compra, count(*)
     from produto
     inner join compra
     on (produto.id_produto = compra.id_produto)
     group by produto.nome, produto.preco, compra.data_compra

     select usuario.nome, telefone.numero_telefone, usuario.email, usuario.cpf, count(usuario.municipio)
     from usuario
     inner join telefone
     on (usuario.id_usuario = telefone.id_usuario)
     group by usuario.nome, telefone.numero_telefone, usuario.email, usuario.cpf
     having count(usuario.municipio) = 1

     select usuario.cpf, produto.nome, sum(compra.quantidade * produto.preco) as total_compra
     from usuario
     inner join compra
     on usuario.id_usuario = compra.id_usuario
     inner join produto
     on (compra.id_produto = produto.id_produto)
     group by usuario.cpf, produto.nome

     select usuario.nome, produto.nome as nome_produto, compra.data_compra, usuario.tipo_logradouro || ' ' || usuario.logradouro ||', ' || usuario.numero as endereco_entrega
     from usuario
     inner join compra
     on (usuario.id_usuario = compra.id_usuario)
     inner join produto
     on (compra.id_produto = produto.id_produto)
     group by usuario.nome, produto.nome, compra.data_compra, usuario.tipo_logradouro, usuario.logradouro, usuario.numero
     order by usuario.nome ASC
     
     
#### 9.8	CONSULTAS COM LEFT, RIGHT E FULL Join (Mínimo 4)<br>

     1 --  mostra todos os nomes de usuarios e nome dos produtos comprados 
     Select usuario.nome, produto.nome
     From usuario
     Inner Join compra
     ON usuario.id_usuario = compra.id_usuario
     RIGHT OUTER Join produto
     ON compra.id_produto = produto.id_produto

    2 --  mostra todos os nomes de usuarios e respectivas quantidade de compras que estao relacionadas a eles 

     Select usuario.nome, compra.quantidade
     From usuario
     LEFT OUTER Join compra
     ON usuario.id_usuario = compra.id_usuario

     3 -- mostra os nomes dos produtos e compra em que eles aparecem 
     
     Select nome,id_compra
     From produto
     FULL OUTER Join compra
     ON produto.id_produto = compra.id_produto
     
     4-- mostra os nomes e cpf dos os empregados que compraram mais de um produto  

     SELECT nome,cpf
     FROM usuario
     FULL OUTER JOIN compra
     ON usuario.id_usuario = compra.id_usuario
     WHERE quantidade > 1



#### 9.9	CONSULTAS COM SELF Join E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join (caso não ocorra na base justificar e substituir por uma view)
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho
    
    1 -- mostra os 3 produtos mais caros
  
       CREATE VIEW mais_caros AS
       Select nome,preco
       From produto 
       Order BY preco DESC
       LIMIT 3
       
    2 -- mostra usuarios que moram no mesmo municipio

     Select usuario1.nome as nome_usuario1, usuario2.nome as nome_usuario2
     From usuario as usuario1
     Inner Join usuario as usuario2
     ON usuario1.municipio = usuario2.municipio
     
     3 -- mostra quantidade vendida
  
     CREATE VIEW quantidade_vendida AS
     SELECT SUM(quantidade)
     FROM compra
     
     4-- mostra o valor total vendido
     
    CREATE VIEW valor_total_vendido AS
    SELECT nome, preco as preco_unitario, quantidade as quantidade_vendida, quantidade * preco as total_vendido
    FROM compra
    INNER JOIN produto
    ON produto.id_produto=compra.id_produto
    
    5-- mostra produto mais caro e o mais barato
    
    CREATE VIEW dados_produtos AS
    SELECT MAX(preco), MIN(preco)
    FROM produto
    
    6- mostra produtos não comprados
    
      CREATE VIEW produtos_nao_comprados AS
      SELECT nome
      FROM produto
      WHERE id_produto NOT IN (SELECT id_produto FROM compra)




   
#### 9.10	SUBCONSULTAS (Mínimo 4)<br>
     a) Criar minimo 1 envolvendo GROUP BY
     b) Criar minimo 1 envolvendo algum tipo de junção
     
    1-- Mostra todos os atributos relativos aos produtos, retornando apenas os registros cujos precos são menores que o valor médio dos precos presentes na tabela produto
    
    Select * From produto
    Where produto.preco < (Select AVG(preco) From produto)
    group by preco

    2-- mostra o nome do usuario e o numero dos produtos que ele comprou, somente para os usuarios que compraram mais de um produto.

    Select usuario.nome, quantidade
    From usuario
    Inner Join compra
    ON usuario.id_usuario = compra.id_usuario
    Where compra.quantidade > 1
    GROUP BY usuario.nome
    
    3-- Mostra todos os atributos relativos aos produtos, retornando apenas os registros cujos precos estão entre 5 - 50 reais.

    Select * From produto
    Where preco > 5
    AND preco < 50

    4-- mostra o nome do usuario e o número de vezes que comprou na loja

    Select nome, COUNT(id_usuario) AS qnt_vezes
    From usuario
    GROUP BY nome


># Marco de Entrega 02: Do item 9.2 até o ítem 9.10<br>

### 10 RELATÓRIOS E GRÁFICOS

#### a) análises e resultados provenientes do banco de dados desenvolvido (usar modelo disponível)
#### b) link com exemplo de relatórios será disponiblizado pelo professor no AVA
#### OBS: Esta é uma atividade de grande relevância no contexto do trabalho. Mantenha o foco nos 5 principais relatórios/resultados visando obter o melhor resultado possível.

    

### 11	AJUSTES DA DOCUMENTAÇÃO, CRIAÇÃO DOS SLIDES E VÍDEO PARA APRESENTAÇAO FINAL <br>

#### a) Modelo (pecha kucha)<br>
#### b) Tempo de apresentação 6:40 

># Marco de Entrega 03: Itens 10 e 11<br>
<br>
<br>
<br> 



### 12 FORMATACAO NO GIT:<br> 
https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>
    
##### About Formatting
    https://help.github.com/articles/about-writing-and-formatting-on-github/
    
##### Basic Formatting in Git
    
    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests
    
    
##### Working with advanced formatting
    https://help.github.com/articles/working-with-advanced-formatting/
#### Mastering Markdown
    https://guides.github.com/features/mastering-markdown/

    
### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.
1. <strong>Caso existam arquivos com conteúdos sigilosos<strong>, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário do git "profmoisesomena", para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.


Link para BrModelo:<br>
http://www.sis4.com/brModelo/download.html
<br>


Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")


