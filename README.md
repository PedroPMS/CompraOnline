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
         id_produto serial not null, 
         nome varchar(15), preco float, 
         primary key(id_produto));

        CREATE TABLE TELEFONE(
         id_telefone serial not null, 
         id_usuario integer, 
         numero_telefone bigint, 
         primary key (id_telefone));

        CREATE TABLE USUARIO(
         id_usuario serial not null, 
         nome varchar(80), 
         cpf bigint, 
         email varchar(100), 
         senha varchar(30), 
         estado varchar(2), 
         municipio varchar(50),
         tipo_logradouro varchar(10), 
         logradouro varchar(50), 
         numero integer, 
         bairro varchar(30), 
         cep integer, 
         primary key(id_usuario));

        CREATE TABLE COMPRA(
         id_compra serial not null, 
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
         id_produto serial not null, 
         nome varchar(15), preco float, 
         primary key(id_produto));

        CREATE TABLE TELEFONE(
         id_telefone serial not null, 
         id_usuario integer, 
         numero_telefone bigint, 
         primary key (id_telefone));

        CREATE TABLE USUARIO(
         id_usuario serial not null, 
         nome varchar(80), 
         cpf bigint, 
         email varchar(100), 
         senha varchar(30), 
         estado varchar(2), 
         municipio varchar(50),
         tipo_logradouro varchar(10), 
         logradouro varchar(50), 
         numero integer, 
         bairro varchar(30), 
         cep integer, 
         primary key(id_usuario));

        CREATE TABLE COMPRA(
         id_compra serial not null, 
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
        INSERT INTO PRODUTO(nome, preco)
        VALUES ('Macacão', 70),('Blusa', 25),('Calça', 300),('Meia', 5), 
               ('Cinto', 25),('Short', 70),('Anoraque', 60),('Avacote', 227),
               ('Hábito', 96),('Jaleco', 286),('Japona', 353),('Beibidol', 130),
               ('Bermuda', 357),('Blazer', 125),('Blusão', 214),('Blusa de lã', 127),
               ('Blêizer', 362),('Boina', 334),('Libré', 367),('Luva', 129),('Manga', 376),
               ('Mantilha', 321),('Mantô', 143),('Maxissaia', 197),('Meia-calça', 332),
               ('Meias', 11),('Mitene', 227),('Botão', 297),('Braguilha', 155),('Brial', 216),
               ('Burca', 238),('Bustiê', 41),('Bódi', 108),('Calça', 302),('Calçado', 179),
               ('Calças', 307),('Calção', 275),('Calções', 380),('Camal', 34),('Camalha', 237),
               ('Camisa', 239),('Camisa social', 264),('Pano', 397),('Pantalonas', 70),('Parangolé', 126),
               ('Parca', 338),('Pareô', 43),('Colete', 343),('Collant', 145),('Colã', 62),('Conjunto', 274),
               ('Coura', 140),('Cueca', 124),('Silaque', 170),('Smoking', 97),('Soquete', 314);

        INSERT INTO USUARIO(nome, cpf, email, senha, estado, municipio, tipo_logradouro, logradouro, numero, bairro, cep)
        VALUES ('Amanda Ferreira', 12345,'amanda@gmail.com', '123@456', 'ES','Vila Velha', 'Rua', 'Olegario Mariano', 1338, 'Soteco', 29106240),
        ('Ana Elisa Rezende', 12120, 'anaelisa@gmail.com', '123@456', 'ES','Serra','Rua','Carapebus', 105, 'Valparaiso', 29165813),
        ('Pedro Paulo Silva', 99999, 'pedro@gmail.com', '123@456', 'ES', 'Vitória', 'Rua', 'Milton Ramalho Simões', 11, 'Jardim Camburi', 29090770),
        ('Lucia Gonçalves',78789, 'lucia@gmail.com','123@456','ES','Vila Velha','Avenida', 'Carlos Lindemberg', 254, 'Araçás',29109600),
        ('Julia Clarindo',81254, 'julia@gmail.com','123@456','ES','Cariacica','Rua', 'Emilio de Abreu', 254, 'Junqueira',29167841),
        ('Paula Abreu',96547, 'paula@gmail.com','123@456','ES','Vila Velha','Avenida', 'Carlos Lindemberg', 256, 'Araçás',29109600),
        ('Joao Junqueira',79996,'joao@gmail.com', '123@456', 'ES', 'Cariacica', 'Rua', 'Nova', 98, 'Orquidea', 29456123),
        ('Viviane Reis',78452, 'viviane@gmail.com','123@456','ES','Vila Velha','Avenida', 'Carlos Lindemberg', 256, 'Araçás',29109600),
        ('Thyago B', 54687, 'thyago@gmail.com', '123@456', 'ES','Serra','Rua','Carapebus', 105, 'Valparaiso', 29165813),
        ('Fernando Henrique', 32659,'fernando@gmail.com', '123@456', 'ES','Vila Velha', 'Rua', 'Olegario Mariano', 1338, 'Soteco', 29106240),
        ('Hardy Teresa', 48173, 'rollin.bradtke@witting.com', 'baumbach.imogene', 'ES', 'Itarana', 'Rua', 'Althea Josefa', 11,'Jardim Camburi', 29008673),
        ('Keely Karlee', 24836, 'bosco.lukas@koelpin.com', 'zion96', 'ES', 'Serra', 'Distrito', 'Bill Lucius', 582,'Maruípe', 29600628),
        ('Wyatt Tillman', 69557, 'cleve03@robel.com', 'jayda.collier', 'ES', 'Serra', 'Travessa', 'Garrison Kieran', 96,'Praia do Canto', 29059309),    
        ('Peggie Marlene', 67568, 'zlakin@gmail.com', 'adelia01', 'ES', 'Colatina', 'Estação', 'Ernestina Emmanuelle', 811,'Jardim da Penha', 29545023),
        ('Jaleel Leone', 25282, 'andreane15@hotmail.com', 'brooklyn94', 'ES', 'Cariacica', 'Travessa', 'Kiara Jules', 374,'Santo Antônio', 29823693),   
        ('Hudson Chet', 59916, 'bonnie.tillman@nienow.com', 'nkirlin', 'ES', 'Vitória', 'Travessa', 'Chelsie Cecelia', 798,'Jardim Camburi', 29914132), 
        ('Missouri Ubaldo', 18277, 'thompson.emma@yahoo.com', 'mandy02', 'ES', 'Colatina', 'Alameda', 'Cierra Johnpaul', 977,'Jardim da Penha', 29168101),
        ('Noel Gregorio', 36006, 'eddie71@hill.org', 'randall.sporer', 'ES', 'Cariacica', 'Rua', 'Jayce Hulda', 747,'Jardim da Penha', 29850758),
        ('Louvenia Irving', 24044, 'destini.block@gmail.com', 'luis.hill', 'ES', 'Vitória', 'Avenida', 'Layne Dejon', 838,'Maruípe', 29818590),
        ('Kari Kody', 62397, 'burley83@trantow.net', 'okessler', 'ES', 'Serra', 'Alameda', 'Elyssa Cynthia', 126,'Santo Antônio', 29421093),
        ('Wade Kendrick', 39256, 'rframi@tromp.net', 'kiana88', 'ES', 'Colatina', 'Alameda', 'Greta Misael', 324,'Goiabeiras', 29019184),
        ('Trevion Gilbert', 56238, 'vandervort.robin@yahoo.com', 'adams.presley', 'ES', 'Cariacica', 'Avenida', 'Bianka Margot', 47,'Praia do Canto', 29042556),
        ('Theron Lea', 34951, 'margarita.quitzon@murphy.com', 'armstrong.vicenta', 'ES', 'Colatina', 'Distrito', 'Jonas Saul', 919,'Praia do Canto', 29681950),
        ('Dena Keyon', 38438, 'rosalind03@gmail.com', 'christelle.roberts', 'ES', 'Pedro Canário', 'Alameda', 'Kaleb Juwan', 23,'Goiabeiras', 29675126),
        ('Kenneth Elmore', 37287, 'celia.terry@wilderman.com', 'oscar.lang', 'ES', 'Itarana', 'Avenida', 'Jaron Bud', 572,'São Pedro', 29069626),
        ('Eladio Francesca', 24148, 'qanderson@doyle.com', 'martina99', 'ES', 'Vila Velha', 'Avenida', 'Luisa Richie', 260,'Jardim Camburi', 29691561),
        ('Derick Colleen', 64537, 'ferne51@hotmail.com', 'harrison.ryan', 'ES', 'Vila Velha', 'Distrito', 'Nola Chanel', 990,'Goiabeiras', 29862035),
        ('Bernie Lessie', 64482, 'tschumm@wintheiser.com', 'jaylan.cassin', 'ES', 'Pedro Canário', 'Alameda', 'Natalia Nelle', 985,'São Pedro', 29393591),
        ('Lavon Agustina', 28773, 'arice@yahoo.com', 'damore.alessandra', 'ES', 'Vitória', 'Rua', 'Myrtle Justyn', 458,'São Pedro', 29389701),
        ('Rae Levi', 59368, 'pgerlach@sawayn.com', 'flittle', 'ES', 'Itarana', 'Avenida', 'Quinton Dayna', 873,'Goiabeiras', 29343750),
        ('Chloe Lucas', 61692, 'nolan.elda@gmail.com', 'royal42', 'ES', 'Colatina', 'Estação', 'Bell April', 583,'Praia do Canto', 29531763),
        ('Nels Keeley', 20995, 'fahey.tony@hotmail.com', 'barmstrong', 'ES', 'Serra', 'Distrito', 'Karley Jalyn', 1000,'Jucutuquara', 29486076),
        ('Napoleon Keon', 63237, 'daron73@gmail.com', 'lwiegand', 'ES', 'Colatina', 'Rua', 'Dina Emerson', 829,'São Pedro', 29271601),
        ('Kathryn Eula', 24430, 'cummings.berneice@jenkins.com', 'ikutch', 'ES', 'Colatina', 'Travessa', 'Joy Maureen', 536,'Jucutuquara', 29459415),
        ('Hannah Sammy', 22742, 'madelynn.smith@mosciski.biz', 'darien44', 'ES', 'Cariacica', 'Travessa', 'Erick Marcel', 595,'Jardim Camburi', 29510613),
        ('Houston Jennie', 61441, 'hickle.berenice@gmail.com', 'gabe.raynor', 'ES', 'Vitória', 'Rua', 'Serena Forest', 50,'São Pedro', 29883816),
        ('Alverta Grayce', 16126, 'lemke.oma@nolan.com', 'feil.roberta', 'ES', 'Colatina', 'Alameda', 'Clemens Gisselle', 434,'Praia do Canto', 29008084),
        ('Elinore Franco', 39632, 'holden.reichel@hotmail.com', 'enos41', 'ES', 'Colatina', 'Rua', 'Amari Caitlyn', 555,'Jucutuquara', 29796417),
        ('Kobe Cleora', 48910, 'emmitt.howell@yahoo.com', 'cadams', 'ES', 'Vitória', 'Distrito', 'Lexus Greta', 312,'Praia do Canto', 29000179),
        ('Uriah Pink', 50452, 'yfay@hotmail.com', 'erling.moore', 'ES', 'Cariacica', 'Travessa', 'Leann Albertha', 758,'Jucutuquara', 29860397),
        ('Anya Rae', 24310, 'orosenbaum@hotmail.com', 'eduardo.oconnell', 'ES', 'Cariacica', 'Alameda', 'Jaylen Violette', 73,'Goiabeiras', 29992643),
        ('Fanny Cloyd', 45012, 'carter.phyllis@parisian.net', 'boyle.mia', 'ES', 'Vitória', 'Estação', 'Herbert Alice', 113,'Santo Antônio', 29813185),
        ('Kacie Rachel', 33472, 'qdickinson@paucek.com', 'diego.stanton', 'ES', 'Cariacica', 'Rua', 'Arvid Danny', 249,'Santo Antônio', 29873295),
        ('Vincent Demetrius', 12503, 'shakira.gerlach@gmail.com', 'carole.kessler', 'ES', 'Vila Velha', 'Estação', 'Shea Eunice', 170,'Praia do Canto', 29765346),
        ('Theo Marcelino', 30095, 'muller.destiney@gmail.com', 'davis.roman', 'ES', 'Itarana', 'Alameda', 'Brandy Glenna', 353,'Praia do Canto', 29067308),
        ('Laron Hazel', 57049, 'estevan.schamberger@gmail.com', 'gottlieb.theresa', 'ES', 'Vitória', 'Rua', 'Kylee Beatrice', 174,'Jardim Camburi', 29062354),
        ('Charity Olga', 26320, 'shayna.zulauf@yahoo.com', 'iframi', 'ES', 'Colatina', 'Distrito', 'Vincent Lexus', 894,'Jardim Camburi', 29176163),
        ('Rylan Jay', 62489, 'alfonzo.nader@yahoo.com', 'halvorson.danyka', 'ES', 'Colatina', 'Rua', 'Carolyne Josiane', 906,'Goiabeiras', 29438786),
        ('Daphney Alverta', 49501, 'willow.spinka@hotmail.com', 'hkeebler', 'ES', 'Vila Velha', 'Estação', 'Rosemary Dave', 602,'São Pedro', 29339513),
        ('Ransom Deja', 51767, 'wlangworth@schumm.com', 'christine.koepp', 'ES', 'Colatina', 'Estação', 'Autumn Morgan', 506,'Jucutuquara', 29825664),
        ('Makenna Ernest', 34237, 'anika45@hotmail.com', 'bruen.wade', 'ES', 'Vila Velha', 'Alameda', 'Mia Dane', 75,'Maruípe', 29248919),
        ('Lisa Justina', 38911, 'jakubowski.heather@gmail.com', 'pdicki', 'ES', 'Vitória', 'Distrito', 'Eladio Malcolm', 103,'Jardim Camburi', 29825836),
        ('Prince Amari', 13581, 'kiarra.strosin@west.com', 'maybell67', 'ES', 'Colatina', 'Avenida', 'Bo Arjun', 42,'Jucutuquara', 29489430),
        ('Timmy Dahlia', 27062, 'ruthe39@schuppe.com', 'aleannon', 'ES', 'Vitória', 'Alameda', 'George Juston', 620,'Jardim da Penha', 29471330),
        ('Tyreek Alejandrin', 30196, 'cristian87@bergstrom.com', 'litzy.collins', 'ES', 'Colatina', 'Rua', 'Melyssa Arielle', 143,'São Pedro', 29541754),
        ('Hayley Dave', 64529, 'sam61@yahoo.com', 'bkutch', 'ES', 'Cariacica', 'Distrito', 'Zelma Stanton', 799,'Jardim Camburi', 29846820),
        ('Lamar Brendan', 32905, 'colt45@yahoo.com', 'viola.heller', 'ES', 'Vila Velha', 'Distrito', 'Blair Daniella', 113,'Goiabeiras', 29234437),
        ('Loraine Earnest', 38376, 'dhowe@ratke.biz', 'lerdman', 'ES', 'Cariacica', 'Rua', 'Yvonne Lilla', 124,'São Pedro', 29938117),
        ('Stone Ardith', 17522, 'acrona@jaskolski.com', 'summer28', 'ES', 'Colatina', 'Estação', 'Weston Sandy', 391,'Goiabeiras', 29143386),
        ('Price Tyshawn', 54557, 'elena.ortiz@gmail.com', 'cale52', 'ES', 'Itarana', 'Avenida', 'Brandy Gilbert', 317,'Jucutuquara', 29901886);

        INSERT INTO TELEFONE(id_usuario, numero_telefone)
        VALUES (1, 985470122),(2, 40028922),(3, 08007777000), 
               (4,965441111), (5,987445632),(6,32180764), 
               (7,20021001),(8, 30100259),(9, 782145215), 
               (10, 54548181),(20, 987697938),(9, 966749190),
               (46, 911006970),(39, 989162928),(49, 951790773),
               (11, 908447176),(42, 996214473),(39, 944663369),
               (28, 995753823),(3, 955704475),(39, 937673200),
               (10, 962344688),(20, 974786886),(17, 923179687),
               (8, 962899636),(10, 960502104),(13, 990713126),
               (4, 978529076),(32, 996383707),(47, 968852085),
               (42, 991704515),(20, 999703283),(27, 971254713),
               (2, 944022538),(46, 914457578),(10, 929726273),
               (3, 953120375),(47, 965688533),(21, 900592189),
               (6, 918137070),(40, 982830443),(37, 991699749),
               (36, 965287476),(41, 953786522),(26, 950283348),
               (25, 990999453),(21, 943688543),(47, 924706862),
               (30, 991653853),(48, 979615422),(1, 908061531),
               (49, 982448829),(43, 943744115),(39, 993889939),
               (2, 917994749),(31, 961673465),(45, 941216329),
               (28, 967675758),(34, 957098046),(15, 910351169);

        INSERT INTO COMPRA(id_produto, id_usuario, data_compra, quantidade)
        VALUES (3, 1, '01-08-2020',1), (4, 2, '01-08-2020', 4),(6, 3, '01-08-2020',2),                
               (5, 4, '01-08-2020',1),(4, 5, '01-08-2020', 1),(3, 6, '01-08-2020', 2),
               (4, 7, '08-28-2020', 1),(6, 8, '08-28-2020', 2),(1, 9, '08-28-2020' , 1),
               (2, 10, '08-28-2020', 2),(22, 35, '2010-06-10', 14),(30, 30, '2010-12-26', 5),
               (23, 49, '2010-05-02', 8),(32, 48, '2011-04-06', 13),(50, 16, '2013-10-03', 13),
               (48, 41, '2019-08-10', 5),(38, 34, '2016-11-02', 8),(32, 45, '2018-10-20', 14),
               (48, 3, '2013-05-01', 14),(30, 45, '2012-02-11', 6),(17, 31, '2012-04-16', 10),
               (30, 20, '2011-04-21', 15),(2, 5, '2014-11-09', 7),(12, 11, '2010-02-23', 14),
               (23, 35, '2010-06-19', 8),(26, 24, '2015-12-03', 14),(48, 23, '2017-07-08', 6),
               (47, 14, '2016-08-19', 9),(17, 7, '2014-12-17', 9),(6, 39, '2012-01-21', 14),
               (22, 46, '2014-08-09', 13),(6, 44, '2013-12-18', 5),(41, 18, '2011-01-28', 14),
               (16, 34, '2012-12-04', 14),(43, 2, '2011-06-09', 12),(10, 34, '2010-05-07', 13),
               (37, 37, '2012-12-07', 2), (50, 3, '2017-01-23', 2),(15, 48, '2011-08-19', 4),
               (23, 30, '2018-08-17', 3),(23, 17, '2010-01-21', 8),(15, 13, '2013-12-17', 13),
               (22, 14, '2013-02-17', 2),(28, 47, '2011-12-02', 2),(9, 13, '2018-06-16', 1),
               (12, 13, '2010-11-17', 10),(25, 33, '2018-06-07', 7),(33, 27, '2017-01-10', 1),              
               (8, 48, '2010-12-05', 6),(34, 50, '2015-04-16', 5),(47, 35, '2013-05-23', 7),    
               (49, 5, '2019-06-18', 7),(19, 37, '2017-02-26', 11),(45, 7, '2015-08-09', 9),
               (3, 16, '2018-01-05', 9),(31, 44, '2017-07-19', 10),(19, 20, '2015-01-07', 4),
               (24, 1, '2012-03-16', 4),(41, 29, '2011-11-02', 12),(5, 18, '2014-02-10', 9);
               
               
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


