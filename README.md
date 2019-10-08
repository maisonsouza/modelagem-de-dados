# Anotações do Curso de Modelagem de Dados Bóson Treinamentos

https://www.youtube.com/watch?v=Q_KTYFgvu1s&list=PLucm8g_ezqNoNHU8tjVeHmRGBFnjDIlxD

## Aula01 - Conceitos de Banco de Dados.
>Dados x Informaçoes (1:31)
Dados são fatos em uma forma primária, que podem ser armazenados em algum meio.
- Exemplo: cpf, Nome, Data

>Informações são os fatos organizados de maneira a produzir significado.
Dados colocados em contexto.
- Exemplo: Lista dos nomes dos clientes ordenados pelo cpf.

* Metadados (3:14)
Dados sobre os dados, utilizados para representações e identificaçao dos dados, garantindo sua consistência e persistência.
São mantidos nos dicionários de dados ou catálogo de dados.

* Banco de Dados.(4:15)

```
Coleção organizada de dados.
Esses dados são organizados para modelar aspectos do mundo real, para que seja possível efetuar processamento que gere informações relevantes para os usuários apartir dos desses dados.
É composto por diversos objetos.
Graficamente é representado por um cilindro.
```

* Aplicações de Banco de dados(6:24)

```
Sistemas bancários
Reserva em hotéis 
Controle de estoque.
Catálogo de livros.
E-commerce
Receita Federal
Youtube
```

* SGBD(8:05)

```
Coleção de softwares que permitem aos usuários criar e manterem um ou mais bancos de dados.
Permitem proteger o banco.
```

* Exemplos de SGDB's(9:07)

```
Oracle
Microsoft SQL Server
MySQL
MongoDB
```

* SGDBR (9:45)
```
Sistema de Gerenciamento de Banco de dados Relacional
Exemplo: SQL Server
```

* Sistema de Banco de Dados(10:40)

```
Usuários, Aplicativos de acesso, SGBD, Banco de dados.
```

* Usuários de Banco de Dados.(11:46)

  * DBA (Cria e gerencia o banco de dados)
  * Projetista/Desenvolvedor (Modelagem e projeto do banco)
  * Usuário Final.(utiliza o banco).
  
* Características e Funcionalidades de Banco de Dados.(12:59)

  * Controle de Redundância.
  Evitar duplicidade dos dados, a informação várias vezes no banco.
  
  * Múltiplas Visões dos Dados.
  Visualizar a informação de ofrmas distintas.
  
  * Controle de Concorrência.
  Gerencia o acesso simultanea dos usuários no banco.
  
  * Backup e Restauração.
  Faz backup e restaura o banco em caso de perdas.
  
  * Autenticação e autorizaçao de acesso.
  
  * Restrições de Integridade.
  Impede que dados sejam cadastrados de maneira indesejada.
  
* Modelos de Banco de Dados.(15:01)
  * Hierárquico.
  ```
  Anos 70, organizados de forma hierarquica.
  Registro pai e registro filho.
  Semelhante a um organograma.
  ```
  
  * Rede.
  
  * ``Relacional``(18:37)
  ```
  Dados separados em entidades com atributos.
  As entidades se relacionam entre si.
  ```
  
  * Orientado a Objetos.
  
  * Não Relacional.
  
## Aula02 - Modelo Relacional

01) Introdução (0:00)
02) Tema da aula: Modelos de Dados (0:07)
03) Modelos (0:15)
```
Um modelo é uma estrutura que ajuda a comunicar os conceitos que estão na mente do projetista.
Deve possuir detalhes suficientes para que um desenvolvedor consiga criar o banco de acordo com a necessidade do projeto.
```
04) Modelagem de Dados (0:26)
```
É o processo de criação de um Modelo de dados para um sistema de informação com a aplicação de técnicas específicas de modelagem.
Quando não criamos o modelo de dados, geralmente criamos um banco com erros.
```
05) Modelos de Dados (2:39)
```
Existem vários tipo de modelo de dados trabalharemos com modelo relacional que é o mais utilizado.
```
06) Modelo Relacional (3:07)
```
Esboçados por E.F.Codd (IBM).
Antigamente utilizava-se modelo hierarquico e de rede.
Dados são organizados em coleções de tabelas bidimensionais.
Essas tabelas são também chamadas de relações.
Baseado em lógica e teoria de conjuntos.
```

a) Componentes do Modelo Relacional (5:13)
```
É composto por relações, operadores, integridade de dados.
```

b) Banco de Dados Relacional (6:05)
```
É uma coleção de relações que são tabelas bidimensionais onde os dados são armazenados.
```
c) Componentes de um Banco de Dados Relacional (7:13)
-Tabelas (7:19)
```
Estrutura básica de armazenamento no SGBDR.
Armazena todos os dados necessários sobre algo do mundo real.
Também chamada de relação.
```
-Tuplas ou linhas/registros (8:02)
```
Representa todos os dados requeridos por uma determinada ocrorrência de entidade em particular.
```

-Colunas (9:21)
```
Unidade que armazena um tipo específico de dado ou não armazenar nada.
```
-Relacionamentos (10:22)
```
Associação entre as entidades(tabelas), conectadas por chaves primárias e estrangeiras.
```
-Outros (Índices, SP, Triggers) (11:44)
```

```
-Chave Primária (11:54)
```
Coluna(atributo) que identifica um registro de forma exclusica na tabela.Exemplo CPF de um cliente.
```
-Chave estrangeira (12:35)
```
Coluna que define como as tabelas se relacionam uma com as outras. Um FK se refere a uma PK ou a uma chave única em outra tabela(ou na mesma tabela)
```
d) Análise de Requisitos (13:07)
```
Nesta fase, são realizadas reuniões para coleta de informações que analisam o que é exigido para o banco de dados a ser criado.
A análise é extramamente importante para o sucesso do projeto do banco de dados.
```
e) Modelo Entidade-relacionamento (MER) (13:44)
```
MER - Cria um diagrama entidade relacionamento apartir das especificações do negócio ou narrativas do usuário.
Permite ilustrar as entidades em um negócio e também relacionamentos entre elas.
Construimos o MER durante a fase de análise no ciclo de vida de desenvolvimento do sistema.
```
-_Entidade (16:46)
```
Algo significativo, sobre o qual devemos possuir informações. Como exemplo temos clientes, funcionários, pedidos e produtos.
```
-Atributo (17:28)
```
Algo que descreve ou qualifica uma entidade 
Exemplo. a entidade cliente possio atributos que descrevem seu nome, endereço, telefone, numero de identificação.
```
-Relacionamento (18:02)
```
Trata-se de uma associação nomeada entre entidades com uma grau de associação.
```
f) Convenções para modelagem (19:15)
```
Nome único, singular, caixa alta
CLIENTE
```
-Entidades (19:25)
```
Nome singular, caixa baixa, atributos obrigatórios ''*'' identificador único marcado com '#'

```
-Atributos (20:00)
```

```
-Relacionamentos (20:24)
```

```
-Cardinalidade (20:41)
```
Cardinalidade significa que cada entidade pode ser ou deve em relação de forma uma e apenas uma ou uma ou mais com outra entidade
```
g) Identificador Único (UID) (21:52)
```
É qualquer combinação de atributos ou relacionamentos que são usados para distinguir ocorrências de uma entidade cada ocorrência da entidade deve ser identificável de forma exclusiva.
```


CONTEÚDO DA AULA 03
01) Introdução (0:00)
02) Modelagem de Dados - Níveis (0:08)
     a) Modelo Conceitual (0:48)
```
Esta é a primeira fase da modelagem, onde representaremos o mundo real por meio de uma visão simplificada dos dados e seus relacionamentos. Assim poderemos determinar quais informações serão armazenadas no BD.
Neste nível o projeto é independente do SGBD.
```
Alto nível
b) Modelo Lógico (3:21)
```
Um modelo lógico possui conceitos que os usuários são capazes de entender, ao mesmo tempo
```
c) Modelo Físico (5:06)
```
Onde se detalha os componentes de estrutura física do banco de dados, incluindo tabela, campos, tipos de valores, restrições.
Ao criarmos o modelo físico poderemos partir para a implementação física do banco de dados.
baixo nível
```
03) Arquitetura de Três Níveis (6:49)
```
Mundo Observado -> 
	Modelo Conceitual ->
		Modelo Lógico ->
    			Modelo Físico.
```
04) Esquema do Banco de Dados (7:45)
```
Definição do banco que foi especificado durante o projeto armazenado no dicionário de dados.
Um esquema raramente muda durante a vida do BD.
```
05) Etapas do Desenvolvimento de um BD (8:34)
```
1. Especificação e Análise de Requisitos
	a) Os requisitos são documentados.
2. Projeto Conceitual
	a)baseado nos requisitos.
3. Projeto Lógico
	a)Expresso em modelo de dados, como o relacional.
4. Projeto Físico.
5. Especificações para armazenar e acessar o banco de dados.
```
a) Análise de Requisitos (8:46)
```

```
b) Projeto Conceitual (9:13)
```

```
c) Projeto Lógico (9:17)
```

```
d) Projeto Físico (9:26)
```

```
06) Tarefas para Modelagem (10:43)
```
As tarefas a seguir devem ser realizadas para que seja possível efetuar modelagem de dados.
```
07) Modelo Entidade-Relacionamento (MER) (11:33)
```
Após o levantamento dos requisitos, estes são transformados em um Modelo-Entidade-Relacionamento(MER), o qual consiste dos seguintes elementos:
Entidades
Relacionamentos
Atributos.
```

AULA04 - Modelo entidade Relacionamento e Diagrama ER
02) Modelo Entidade-Relacionamento (MER) (0:08)
```
Também conhecido como MER, trata-se de um modelo conceitual usado para descrever objetos envolvidos no domínio de um sistema a ser constituído incluindo seus atributos.
Diagramas Entidade Relacionamento(DER)
```
02.1) Entidades (1:13)
```

```
a) MER (1:25)
```
Criado pelo Dr. Peter chen, criador do Modelo ER.
```

b) DER (1:45)
```
Representação gráfica associada ao MER(ou a parte dele).
```
c) Modelo e Diagrama (2:19)
```

```
d) Componentes do DER (3:00)
```
Retângulo, Elipses. Losangose linhas.
- Entidade: Retângulos
- Atributo: Elipses
- Relacionamento: Losangos
- Linhas: Ligações
```
e) Exemplo de DER (4:28)

![](https://quantum2013.files.wordpress.com/2013/08/der-por-enquanto1.jpg?w=584&h=264)

```

```

# Modelagem de Dados - O que são Entidades

01) Introdução ([0:00](https://www.youtube.com/watch?v=poeUGQl52YI&list=PLucm8g_ezqNoNHU8tjVeHmRGBFnjDIlxD&t=0s))

02) Entidades([0:08](https://www.youtube.com/watch?v=poeUGQl52YI&list=PLucm8g_ezqNoNHU8tjVeHmRGBFnjDIlxD&t=8s))
``` 

```

​     a) Regras para nomear entidades ([2:24](https://www.youtube.com/watch?v=poeUGQl52YI&list=PLucm8g_ezqNoNHU8tjVeHmRGBFnjDIlxD&t=144s))
``` 
Usando substantivos que representam de forma clara e objetiva sua função, geralmente no singular.
Dentro de retângulos contendo o nome da entidade.
Devem começar com uma letra
Não podem ter espaços ou alguns caracteres especiais.
Alguns caracteres como $,#,+ são permitidos em alguns bancos de dados.
Os nomes das colunas devem ser únicos dentro de uma tabela.
Os nomes de entidades/tabelas devem ser únicos dentro de um esquema.
```
​     b) Instância de Entidade ([7:35](https://www.youtube.com/watch?v=poeUGQl52YI&list=PLucm8g_ezqNoNHU8tjVeHmRGBFnjDIlxD&t=455s))
``` 
Entidade é uma receita ou planta.
É uma ocorrência específica de uma entidade.
```

Modelagem de Dados - O que são Atributos

CONTEÚDO DA AULA 06...

01) Introdução (0:00)

02) Atributos(0:08)
CONTEÚDO DA AULA 06...
01) Introdução (0:00)
02) Atributos(0:08)
     a) Representando Atributos (1:12)
     b) Tipos de Atributos (2:35)
         - Atributo Simples/Atômico (3:18)
         - Atributo Composto (4:20)
         - Atributo Multivalorado (5:53)
         - Atributo Determinante (7:04)
         - Atributos Identificadores ("Chaves") (9:05)
    c) Exemplos de Representação de Entidades e Atributos (11:05)
