# :notebook: :pencil2: Anotações do Curso de Modelagem de Dados Bóson Treinamentos

https://www.youtube.com/watch?v=Q_KTYFgvu1s&list=PLucm8g_ezqNoNHU8tjVeHmRGBFnjDIlxD

## Aula01 - Conceitos de Bancos de Dados
* Dados x Informaçoes (1:31)

```
Dados são fatos em uma forma primária, que podem ser armazenados em algum meio.
Exemplo: CPF, Nome, Data
```
```
Informações são os fatos organizados de maneira a prozir significado.
Dados colocados em contexto.
Exemplo: Lista dos nomes dos clientes ordenados pelo cpf
```

* Metadados (3:14)
```
Dados sobre os dados, utilizados para representaçÃO e identificaçao dos dados, garantindo sua consistência e persistência.
São mantidos nos dicionários de dados ou catálogo de dados
```

* Banco de Dados (4:15)
```
Coleção organizada de dados.
Esses dados são organizados para modelar aspectos do mundo real, para que seja possível efetuar processamento que gere informações relevantes para os usuários apartir desses dados.
É composto por diversos objetos COMO tabelas, esquemas, visões, consultas, relatórios, procedimentos, triggers.
Graficamente é representado por um cilindro.
```

* Aplicações de Banco de dados (6:24)
```
Bancos de dados encontram-se em ínumeras áreas.
* Sistemas bancários
* Reserva em hotéis 
* Controle de estoque.
* Catálogo de livros.
* E-commerce
* Receita Federal
* Youtube
```

* SGBD(8:05)
```
Coleção de softwares que permitem aos usuários criar e manterem um ou mais bancos de dados.
Permitem proteger o banco.
São usados nas tarefas de definição, construção, manipulação e compartilhamento dos bancos de dados entre as aplicações e usuários.
Permitem proteger o banco de dados e mantê-lo ao longo do tempo.
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
Usuários, Aplicativos de acesso, SGBD, Banco de dados e metadados.
```

* Usuários de Banco de Dados.(11:46)
```
* DBA (Cria e gerencia o banco de dados)
* Projetista/Desenvolvedor (Modelagem e projeto do banco)
* Usuário Final.(utiliza o banco).
```

* Características e Funcionalidades de Banco de Dados.(12:59)
```
* Controle de Redundância.
Evitar duplicidade dos dados, a informação várias vezes no banco.

* Múltiplas Visões dos Dados.
Visualizar a informação de formas distintas, dependendo da necessidade.

* Controle de Concorrência.
Gerencia o acesso simultâneo dos usuários no banco.

* Backup e Restauração.
Faz backup e restaura o banco em caso de perdas.

* Autenticação e autorizaçao de acesso.
Somente pessoas autorizados podem ter acesso aos dados.

* Restrições de Integridade.
Impede que dados sejam cadastrados de maneira indesejada.
```

* Modelos de Banco de Dados.(15:01)
```
Antigamente os dados eram armazenados em fichas.
Não havia computadores para armazenamento de dados e informação.
```

* Hierárquico.
```
Anos 70, organizados de forma hierarquica.
Registro pai e registro filho.
Semelhante a um organograma.
```

* Rede.
```
Os dados são organizados em tipos e ligações entre dois registros.
```

* `Relacional`(18:37)
```
Dados separados em entidades com atributos.
As entidades se relacionam entre si.
```
