<img src='/img/logo.png' alt='logo da empresa' width='50px' heidth='50px'/>

# *FIBONACCI MANAGEMENT SYSTEM*

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
| BENEFÍCIOS ESPERADOS |* Aumento no lucro da biblioteca real;<br/>* Novos alcances em mais leitores;<br/>* Menor curso de operação;<br/>* Mais reconhecimento;<br/>*|
| INÍCIO E TÉRMINO PREVISTOS | 07/2025 - 07/2026 |

[ [INÍCIO](#fibonacci-management-system) ]

# INTRODUÇÃO

## PROPÓSITO DESTE DOCUMENTO

Este documento destina-se aos clientes, engenheiros, gerentes e demais stakeholders deste projeto. O propósito deste documento é apresentar a descrição dos serviços e funções que o sistema **_Fibonacci Management System_** deve prover, bem como as suas restrições de operação e propriedades gerais, a fim de ilustrar uma descrição detalhada do sistema para um auxílio durante as etapas de análise, projeto e testes. O documento especifica todos os requisitos funcionais e não funcionais do sistema e contém a prototipagem, além de diagramas UML que foram construídos levando-se em conta as funcionalidades identificadas durante a fase de concepção do sistema.

[ [INÍCIO](#fibonacci-management-system) ]

# DESCRIÇÃO GERAL

## Usuários do sistema
|USUÁRIO|DESCRIÇÃO|
|:---|:---|
|**Usuário Padrão:**|Realizam as tarefas comuns a todos os usuários, tal como: logar e enviar mensagens. Todos demais usuários estendem as funcionalidades do UsuárioPadrão|
|**Administrador:**|Responsáveis pelo gerenciamento das entidades pertinentes à instituição e pela alocação de outros administradores|
|**Coordenador:**|Responsáveis pela aprovação de disciplinas, turmas e matrículas realizadas pela secretaria do curso, além de ser responsável pela alocação da secretaria|
|**Secretaria:**|Responsáveis pelo cadastramento de disciplinas e turmas, pela alocação de professores e monitores de um curso e matrículas dos alunos|
|**Professor:**|Responsáveis pela criação do programa da disciplina através de ferramentas de planejamento e criação de atividades|
|**Aluno:**|Seguem o programa da disciplina criada pelo professor, tendo como apoio ferramentas de comunicação, tal como: chat e fórum|


[ [INÍCIO](#fibonacci-management-system) ]

# Metodologia Adotada no Desenvolvimento

[ [INÍCIO](#fibonacci-management-system) ]

# Requisitos do Software

A especificação dos requisitos deste documento deve seguir as recomendações da norma IEEE Std-830-1998, levando em conta as recomentações do documento de [características dos requisitos](caracteristicas_requisitos.md).

## Requisitos Funcionais

A tabela a seguir contém a relação dos Requisitos Funcionais elicitados, com as colunas: identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO |
:---|:---|:---|
|RF-001 |Cadastrar usuário na plataforma | Todos os usuários da plataforma precisam se registrar, fornecendo dados pessoais mínimos como e-mail, senha, nome completo, CPF, data de nascimento e endereço. O registro pode ser feito por meio de um formulário ou integração com contas do Google, Microsoft, Facebook ou login do servidor público. Cada usuário terá um perfil de acesso específico, que pode ser ajustado ou expandido conforme as necessidades surgirem. |
|RF-002 | Publicar, manter e excluir documentos | A ferramenta permite que os usuários façam upload de materiais textuais em vários formatos, como OpenDocument, Microsoft Office, Adobe PDF, Plain Text e RichText Format, para os espaços digitais existentes.|
|RF-003 | Excluir conta do usuário | A funcionalidade permite que os usuários excluam suas contas da plataforma diretamente na página de perfil, com uma confirmação simples via palavra-chave. Os dados da conta são excluídos imediatamente após a confirmação.|
|RF-004 | Crias, manter e excluir salas de chat online (mensagens instantâneas) | Os administradores dos espaços digitais podem criar, manter e excluir salas de bate-papo online, onde os participantes interagem por meio de mensagens de texto. As salas podem ser configuradas para permitir apenas convidados ou serem abertas para usuários cadastrados na plataforma.|
|RF-005 | Criar, manter e excluir “subsites” | A plataforma permite a criação de "subsites", que são seções independentes com seus próprios espaços digitais, comunidades e recursos. Apenas administradores e gestores podem criar subsites, que podem ter recursos exclusivos ou compartilhados com a plataforma principal e também podem personalizar seus temas gráficos.|
|RF-006 | Buscar conteúdo na plataforma | Permite aos usuários localizar conteúdos diversos na plataforma, tais como postagens em fóruns, comunidades, pessoas, documentos, imagens, vídeos, web rádios etc. A busca deve ser realizada por padrão no contexto onde se encontra o usuário, mas sendo possível expandi-lo para toda a plataforma. Os resultados exibidos são apenas os que o usuário é capaz de acessar. A consulta deve reconhecer os principais operadores de busca, tais como “AND”, “OR”, “XOR”, “NOT”. Deve ainda existir uma opção de consulta avançada, onde é possível determinar critérios adicionais, como tipos de conteúdo, intervalo de tempo, nome de usuário etc.|
|RF-007 | Cadastrar perfis de usuários | Os perfis de usuários são definidos pelo Governo do Estado e configurados pela administração da plataforma, permitindo incluir perfis de acesso com permissões específicas. Existem perfis pré-existentes, como Administrador, Gestor, Governo, OSC e Cidadão, além de perfis para espaços digitais, como Administrador, Moderador e Padrão. O perfil "Cidadão" é o padrão para novos usuários, com permissões mínimas.|
|RF-008 | Identificar-se (login) na plataforma | A plataforma requer autenticação do usuário por meio de login e senha, com opção de login via Google, Facebook, Microsoft e, se possível, Governo do Ceará. O formulário de login inclui campos para nome de usuário e senha, além de um mecanismo de segurança Captcha para proteger os usuários.|


## Requisitos Não Funcionais
A tabela a seguir contém a relação com os Requisitos Não Funcionais identificados, contendo identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO |
|:---|:---|:---|
|RNF-001 |Nome do Requisito |Descreva aqui as informações sobre o requisito |
|RNF-002 |Nome do Requisito |Descreva aqui as informações sobre o segundo requisito |


[ [INÍCIO](#fibonacci-management-system) ]


# Prototipagem

[Protótipo criado no FIGMA em 2022 por estudantes](https://www.figma.com/fi0,
le/iNC7wyX9zP7Kmn3BhiCFGf/Fals6Hood-(Prot%C3%B3tipo-criado-por-estudantes-em-2022)?node-id=0%3A1&t=B16hgeZP3MSURCCa-1)

![Imagem do Protótipo](/img/home.png)

[ [INÍCIO](#fibonacci-management-system) ]


# Diagrama de Classes

![Diagrama de Classes](/img/CDModelo.png)

[ [INÍCIO](#fibonacci-management-system) ]


# REFERÊNCIAS

Esta subseção apresenta as referências aos documentos que utilizamos no auxílio à construção deste documento.
* [UML](https://www.omg.org/spec/UML/2.5/About-UML/)
* [Práticas para Especificação de Requisitos IEEE-830](https://ieeexplore.ieee.org/document/720574)
