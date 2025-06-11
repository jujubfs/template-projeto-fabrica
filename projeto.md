<img src='/img/logo.png' alt='logo da empresa' width='50px' heidth='50px'/>

# *BIBLIOTECA*

# PROJETO DE SOFTWARE

## *Stakeholders*
|NOME|CARGO|E-MAIL|
|:---|:---|:---|
|Julia Vitória Bitencourt da Fonseca Silva|Gerente de Projeto|julia.bitencourt@estudante.ifro.edu.br|
|Maria Vitória Oliveira Teixeira|Full Stack|v.maria@estudante.ifro.edu.br|
|Ana Paula Clemente del Barco|Full Stack|paula.barco@estudante.ifro.edu.br|
|Yasmin Vitória Paiano|Full Stack|yasmimvitoriapaiano@gmail.com|
|Elyã Zam da Silva Sousa|Full Stack|elyazssousa@gmail.com|
|Nícollas Piettro Damatta Silva|Full Stack|damatta.nicollas@estudante.ifro.edu.br|
|Davi Valadão Fantin|Full Stack|v.davi.f10@gmail.com|


# Sumário

* [RESUMO DO PROJETO](#resumo-do-projeto)
* [INTRODUÇÃO](#introdução)
  * [PROPÓSITO DESTE DOCUMENTO](#propósito-deste-documento)
* [DESCRIÇÃO GERAL](#descrição-geral)
  * [USUÁRIOS DO SISTEMA](#usuários-do-sistema)
  * [ABRANGÊNCIA E SISTEMAS SIMILARES](#abrangência-e-sistemas-similares)
  * [SUPOSIÇÕES E DEPENDÊNCIAS](#suposições-e-dependências)
* [METODOLOGIA ADOTADA NO DESENVOLVIMENTO](#metodologia-adotada-no-desenvolvimento)
* [REQUISITOS DO SOFTWARE](#requisitos-do-software)
  * [REQUISITOS FUNCIONAIS](#requisitos-funcionais)
  * [REQUISITOS NÃO FUNCIONAIS](#requisitos-não-funcionais)
* [PROTOTIPAGEM](#prototipagem)
* [DIAGRAMA DE CLASSES](#diagrama-de-classes)
* [REFERÊNCIAS](#referências)


# RESUMO DO PROJETO
| ITEM | DESCRIÇÃO|
|:---|:---|
| NOME DO PROJETO | Biblioteca |
| GERENTE DO PROJETO | Julia Vitória Bitencourt da Fonseca Silva |
| PRINCIPAL OBJETIVO | Desenvolver um software que possa representar a biblioteca de forma online, afim de trazer mais acessibilidade as pessoas. |
| BENEFÍCIOS ESPERADOS |* Aumento no lucro da biblioteca real;<br/>* Novos alcances em mais leitores;<br/>* Menor curso de operação;<br/>* Mais reconhecimento;<br/>|
| INÍCIO E TÉRMINO PREVISTOS | 07/2025 - 07/2026 |

[ [INÍCIO](#Bibliotea) ]

# INTRODUÇÃO

## PROPÓSITO DESTE DOCUMENTO

Este documento destina-se aos clientes, engenheiros, gerentes e demais stakeholders deste projeto. O propósito deste documento é apresentar a descrição dos serviços e funções que o sistema **_Biblioteca_** deve prover, bem como as suas restrições de operação e propriedades gerais, a fim de ilustrar uma descrição detalhada do sistema para um auxílio durante as etapas de análise, projeto e testes. O documento especifica todos os requisitos funcionais e não funcionais do sistema e contém a prototipagem, além de diagramas UML que foram construídos levando-se em conta as funcionalidades identificadas durante a fase de concepção do sistema.

[ [INÍCIO](#Biblioteca) ]

# DESCRIÇÃO GERAL

## Usuários do sistema
|USUÁRIO|DESCRIÇÃO|
|:---|:---|
|**Usuário Padrão:**|Realizam as tarefas comuns a todos os usuários, tal como: logar e comprar/alugar/vender livros. Todos demais usuários estendem as funcionalidades do UsuárioPadrão.|
|**Administrador:**|Responsáveis pelo gerenciamento das entidades pertinentes à biblioteca/livraria e pela alocação de outros administradores.|
|**Assistência telefônica:**|Responsáveis pelo cadastramento de livros e autores, e auxiliam na definição de preços.|


[ [INÍCIO](#Bibliotea) ]

# Metodologia Adotada no Desenvolvimento

[ [INÍCIO](#Bibliotea) ]

# Requisitos do Software

A especificação dos requisitos deste documento deve seguir as recomendações da norma IEEE Std-830-1998, levando em conta as recomentações do documento de [características dos requisitos](caracteristicas_requisitos.md).

## Requisitos Funcionais

A tabela a seguir contém a relação dos Requisitos Funcionais elicitados, com as colunas: identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO | IMPORTÂNCIA |
|:---|:---|:---|:---|
|RF-001 |Cadastrar usuário na plataforma | Todos os usuários da plataforma precisam se registrar, fornecendo dados pessoais mínimos como e-mail, senha, nome completo, CPF, data de nascimento e endereço. O registro pode ser feito por meio de um formulário ou integração com contas do Google, Microsoft, Facebook ou login do servidor público. Cada usuário terá um perfil de acesso específico, que pode ser ajustado ou expandido conforme as necessidades surgirem. | Alta |
|RF-002 | Publicar, manter e excluir documentos | A ferramenta permite que os usuários façam upload de materiais textuais em um formato, como PDF, para os espaços digitais existentes.| Alta |
|RF-003 | Excluir conta do usuário | A funcionalidade permite que os usuários excluam suas contas da plataforma diretamente na página de perfil, com uma confirmação simples via palavra-chave. Os dados da conta são excluídos imediatamente após a confirmação.| Média |
|RF-004 | Buscar conteúdo na plataforma | Permite aos usuários localizar conteúdos diversos na plataforma, tais como postagens em fóruns, comunidades, pessoas, documentos, imagens, vídeos, web rádios etc. A busca deve ser realizada por padrão no contexto onde se encontra o usuário, mas sendo possível expandi-lo para toda a plataforma. Os resultados exibidos são apenas os que o usuário é capaz de acessar. A consulta deve reconhecer os principais operadores de busca, tais como “AND”, “OR”, “XOR”, “NOT”. Deve ainda existir uma opção de consulta avançada, onde é possível determinar critérios adicionais, como tipos de conteúdo, intervalo de tempo, nome de usuário etc.| Alta |
|RF-005 | Cadastrar perfis de usuários | Os perfis de usuários são definidos pelo Governo do Estado e configurados pela administração da plataforma, permitindo incluir perfis de acesso com permissões específicas. Existem perfis pré-existentes, como Administrador, Gestor, Governo, OSC e Cidadão, além de perfis para espaços digitais, como Administrador, Moderador e Padrão. O perfil "Cidadão" é o padrão para novos usuários, com permissões mínimas.| Alta |
|RF-006 |Cadastrar livros | O requisito funcional de Cadastrar Livros permite que usuários autorizados insiram, editem e excluam informações de livros, incluindo título, autor, editora e ISBN, facilitando a gestão e busca de livros de forma eficiente. | Alta |
|RF-007 |Cadastrar autores | O requisito funcional de Cadastrar Autores permite que usuários autorizados registrem informações sobre autores, incluindo nome, biografia e obras publicadas, possibilitando a gestão e busca eficiente de dados sobre escritores. | Alta |
|RF-008 |Cadastrar gêneros | O requisito funcional de Cadastrar gêneros permite que usuários autorizados registrem informações sobre os gêneros dos livros, possibilitando a gestão e busca eficiente de dados sobre so gêneros. | Alta |
|RF-009 | Pesquisar Livros | Permite que usuários busquem livros por título, autor, gênero ou outras palavras-chave. | Média |
|RF-010 | Gerenciar empréstimos | Permite que usuários autorizados registrem e gerenciem empréstimos de livros, incluindo data de devolução e status | Média | 
|RF-011 | Visualizar Catálogo | Permite que usuários visualizem o catálogo de livros disponíveis na biblioteca. | Alta | 
|RF-012 | Gerenciar perfil do usuário | Permite que usuários visualizem e editem suas informações de perfil, incluindo histórico de empréstimos. | Média |
|RF-013 | Notificações | Envia notificações para usuários sobre datas de devolução, disponibilidade de livros reservados, etc. | Baixa |
|RF-014 | Adiministração de conteúdo | Permite que administradores gerenciem o conteúdo do site, incluindo notícias, eventos e anúncios. | Alta |
|RF-015 | Processamento de pagamento | Integração com gateways de pagamento e suporte a diferentes métodos de pagamento. | Alta |
|RF-016 | Gestão de carrinho de compras | Adicionar, remover e visualizar itens no carrinho. | Alta |
|RF-017 | Confirmação de pagamento | Envio de confirmação de pagamento e atualização do status de pagamento. | Alta |
|RF-018 | Gestão de cupons e promoções | Aplicação e validação de cupons e promoções. | Alta |
|RF-019 | Segurança de pagamento |  Conformidade com padrões de segurança e criptografia de dados de pagamento. | Alta |
|RF-020 | Gestão de Reembolsos e Cancelamentos | Opção de solicitar reembolso ou cancelar compra e processamento de reembolsos. | Alta |
|RF-021 | Histórico de pagamentos | Visualização do histórico de pagamentos e acesso a recibos e faturas. | Alta |
|RF-022 | Pedidos realizados | Mostra ao usuário os produtos que ele já comprou | Média |

## Requisitos Não Funcionais
A tabela a seguir contém a relação com os Requisitos Não Funcionais identificados, contendo identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO | IMPORTÂNCIA |
|:---|:---|:---|:---|
|RNF-001 | Desempenho | O site deve carregar rapidamente e lidar com usuários simultâneos sem perda de desempenho. | Alta |
|RNF-002 | Segurança | O site deve proteger informações pessoais e ser protegido contra ameaças. | Alta |
|RNF-003 | Usabilidade | O site deve ser fácil de navegar e acessível para usuários de diferentes níveis de habilidade. | Alta |
|RNF-004 | Compatibilidade | O site deve ser compatível com diferentes navegadores e dispositivos. | Alta |
|RNF-005 | Manutenção | O site deve ser fácil de atualizar e manter, com backups automáticos. | Média |
|RNF-006 | Acessibilidade | O site deve seguir diretrizes de acessibilidade web para garantir acesso a usuários com deficiências. | Alta |
|RNF-007 | Recursos | O site deve utilizar recursos de produção como: MySql, JavaScript, CSS e Html. | Alta |

[ [INÍCIO](#Bibliotea) ]


# Prototipagem

[Protótipo criado no FIGMA em 2025 por estudantes](https://www.figma.com/fi0,
le/iNC7wyX9zP7Kmn3BhiCFGf/Fals6Hood-(Prot%C3%B3tipo-criado-por-estudantes-em-2022)?node-id=0%3A1&t=B16hgeZP3MSURCCa-1)

![Imagem do Protótipo](/img/home.png)

[ [INÍCIO](#Bibliotea) ]


# Diagrama de Classes

Classes

- **Livro:** representa um livro na biblioteca
    - Atributos: ID_livro, titulo, autor, editora, ano_de_publicacao, isbn, preco, categoria, status
- **Autor:** representa um autor de livros
    - Atributos: ID_autor, nome, biografia, dataNascimento, dataFalecimento
- **Usuário:** representa um usuário da biblioteca
    - Atributos: nome, e-mail, senha, ID_usuario
- **Carrinho:** representa um carrinho de compras de um usuário
    - Atributos: ID_carrinho, ID_usuario, listaLivros
- **Pedido:** representa um pedido de compra de um usuário
    - Atributos: lista_de_livros, total, status_de_pagamento
- **Pagamento:** representa um pagamento de um pedido
    - Atributos: metodo_de_pagamento, status_de_pagamento, valor
- **Empréstimo:** representa um empréstimo de um livro
    - Atributos: livro, usuario, data_de_devolucao

Relações

- Um livro é escrito por um autor (1:1)
- Um autor pode escrever muitos livros (1:N)
- Um usuário pode ter muitos carrinhos (1:N)
- Um carrinho pertence a um usuário (1:1)
- Um pedido é feito por um usuário (1:1)
- Um pedido pode conter muitos livros (1:N)
- Um pagamento é feito para um pedido (1:1)
- Um empréstimo é feito por um usuário e envolve um livro (1:1)

![Diagrama de Classes](/img/Diagrama%20de%20Classe%20-%201.jpeg)

[ [INÍCIO](#Bibliotea) ]


# REFERÊNCIAS

Esta subseção apresenta as referências aos documentos que utilizamos no auxílio à construção deste documento.
* [UML](https://www.omg.org/spec/UML/2.5/About-UML/)
* [Práticas para Especificação de Requisitos IEEE-830](https://ieeexplore.ieee.org/document/720574)
