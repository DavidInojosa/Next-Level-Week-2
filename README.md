# **Next Level Week #02 | Proffy**

Prática da Next Level Week #02 | [Rocketseat][Rocketseat]

![Banner topo][Banner topo]

  

## **Introdução**

___
  

### Projeto **Proffy**

Esse repositório contempla a prática proposta na **segunda edição da `<nwl/>` (NextLevelWeek)**, cujo projeto se chama **Proffy**.

![Proffy](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F3368c282-bf94-49bb-bc6b-905542231e2c%2FPattern.png?table=block&id=3d5f45f5-4ec5-4ef9-b210-3565b7cce4e1&width=3840&cache=v2)

> O nome **Proffy** é uma homenagem ao dia 06 de Agosto, Dia dos Professores.

O projeto chama-se **Proffy** e consiste numa plataforma de _e-learning_, onde se conecta alunos e professores numa plataforma de estudos _online_ com opções de criar perfil, cadastro de matérias, horários e valores de aula, buscar por registro de professores (com filtros por horário e matéria) e agendar aulas (não contempla vídeo chamadas). Os dados serão salvos (_storage_) do lado do cliente. Utilizamos o conceito _bubble first_ (_mobile first_), privilegiando os dispositivos _mobile_.

### Configuração do Ambiente

Antes de iniciarmos precisamos garantir que temos todas as ferramentas necessárias disponíveis em nosso ambiente local. A [Rocketseat][Rocketseat] preparou um [documento](https://www.notion.so/Configurando-Ambiente-NLW-98a471ad3cb6448284b8ceed31c45767) com o passo a passo para realizarmos essa configuração - seja para [instalar as dependências](https://www.notion.so/Instala-o-3d8bc65b8a0f48249bf3037156eb0a15), seja para [atualizá-las](https://www.notion.so/Atualiza-o-138506d91f2d422da44f5ccd4354186b), além de um documento com alguns dos [erros mais comuns](https://www.notion.so/Tive-problemas-e-agora-7190da61cb234af88e5861d5d2897ad7) que podem ocorrer durante essa configuração.

Antes de prosseguir, execute os seguintes comandos no terminal, para garantir que estamos com a mesma versão do _[node][node]_ e do _[npm][npm]_:

``` sh
node -v
// deve retornar v12.8.3

npm -v
// deve retornar 6.14.6
```

### Layout

Garanta que possui acesso aos arquivos de _layout_ do projeto no [Figma][Figma] para ter uma melhor visão do que será construído.

### Funcionalidades

##### Conexões

* Rota de listagem de conexões realizadas (operação de soma dos registros)

* Rota de criação de nova conexão (ativada quando clicarem em __Entrar em contato__)

##### Aulas

* Rota de listagem de aulas [filtros por matéria, dia da semana e hora]

* Rota de Criação de nova aula

### Tecnologias

Confira as principais tecnologias utilizadas no projeto:

##### React

[React][React] é uma **biblioteca de construção de interfaces SPA que via otimizar a experiência do usuário**. Também existem 'sub pacotes' do [React][React], de acordo com o ambiente da aplicação - veja alguns dos principais:

| ambiente | 'sub pacote' |
| ----- | ----- |
| Web | [ReactJS][ReactJS] |
| Mobile App | [React Native][React Native] | [Não terminei o Mobile App - DavidInojosa] |

Independentemente do 'sub pacote', sempre utilizaremos o **[React][React]**. O [React][React] também utiliza bibliotecas adicionais para integrar-se às interfaces de acordo com o ambiente. Por exemplo, na web utilizamos o [ReactJS][ReactJS] com o [ReactDOM][ReactDOM]. Já para _apps mobile_ utilizamos o [ReactNative][ReactNative] com uma biblioteca adicional também chamada de [ReactNative][ReactNative].

##### Node.js

É uma plataforma que nos permite utilizar o mesmo JavaScript (puro ou com ReactJS, ...) no back-end.

* _Non-blocking IO_: conseguimos controlar a assincronicidade

* Streams (nos permite consumir dados no estilo '_LazyLoad_') e WorkerThreads (nos permite trabalhar o _core_)

##### TypeScript

O [TypeScript][TypeScript] é uma extensão do JavaScript que utiliza a tipagem que facilita a manutenção do código e garante a consistência de nossas soluções, pois captura um erro antes mesmo de sua execução. Também possui recursos para IDEs que otimizam o desenvolvimento.

##### Knex

O Knex é um _query builder_, que possibilita escrevermos as _queries_ de forma mais simples, em JavaScript.

##### SQLite

O _sqlite3_ é um pacote de banco de dados mais leve, não requer instalações na máquina. Usaremos a sintaxe do _knex_ para trabalharmos com o _sqlite3_.
___
  
