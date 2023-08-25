# O que é o Nest?

Nestjs é um framework para construção de aplicações servidoras utilizando Node.js. 
Nest pode trabalhar com TypeScript e Javascript, combinando elementos de POO,
Programação Funcional e Programação Funcional Reativa.

O Nest busca resolver o problema de arquitetura dos frameworks JavaScript, sendo fortemente 
inspirado no Angular.

O Nest usa uma estrutura através de modulos.

## Sobre os Módulos

O arquivo app.module.ts é o módulo raiz da aplicação.
O arquivo main.ts é o arquivo de entrada que usa a função NestFactory para criar as instâncias do aplicativo.
Os controladores sempre pertencem a um modulo.

## Middlewares

Middlewares são funções chamadas antes dos manipuladores de rota.
As funções de middleware têm acesso aos objetos request e response e a função next() - próxima função -  de middleware no ciclo de request-response do aplicativo. O próximo função middleware é geralmente indicada por uma variável chamada next.
## Providers

Os providers são classes JavaScript simples que são declaradas como providers em um módulo.

*Providers são como services*

Os providers (fornecedores - de serviços em geral) são um conceito fundamental no nest.
A principal ideia é que eles podem ser injetados como um dependência, criando vários relacionamentos entre os objetos.

Os controladores devem lidar com solicitações HTTP e delegar tarefas mais complexas para os providers.

Os provider são inicializados junto com o aplicativo e destruidos ao final dele. Esse comportamento pode ser modificado.

## Módulos

Os módulos são classes anotadas com o decorator @Module. Eles provem os metadados para organizar a estrutura dos aplicativos.

Cada aplicação possui pelo menos um módulo, o módulo raiz. O módulo raiz é o ponto de partida que o Nest usa para criar o gráfico de aplicação.
A arquitetura dos aplicativos em geral possuem vários módulos, cada um encapsulando um conjunto de recursos.

**Módulos de recursos** 
Um módulo de recurso simplesmente organiza o código relevante para um recurso específico, 
mantendo o código organizado e estabelecendo limites.


## DTO - Data Transfer Object

Um DTO é um objeto que define como os dados serão enviados pela rede.

## Geral

Para criarmos uma nova rota precisamos criar o controlador e adicionar ele no modulo

## Monorepo

Padrão em que utilizamos um único repositório para guardar todos os projetos.

Vantagens:
- Ambiente de desenvolvimento
- Reutilização de código
- Gerenciamento de dependências
- Gerenciamento de versões

Desvantagens:
- CI/CD: podem se tornar complexos, não é trivial identificar qual aplicação está sendo alterada, dificultando a automatização.
- Segurança: todos os desenvolvedores tem acesso a tudo.