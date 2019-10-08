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
