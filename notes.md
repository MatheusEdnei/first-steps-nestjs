# O que é o Nest?

Nestjs é um framework para construção de aplicações servidoras utilizando Node.js. 
Nest pode trabalhar com TypeScript e Javascript, combinando elementos de POO,
Programação Funcional e Programação Funcional Reativa.

O Nest busca resolver o problema de arquitetura dos frameworks JavaScript, sendo fortemente 
inspirado no Angular.

O Nest usa uma estrutura através de modulos.

# Sobre os Módulos

O arquivo app.module.ts é o módulo raiz da aplicação.
O arquivo main.ts é o arquivo de entrada que usa a função NestFactory para criar as instâncias do aplicativo.
Os controladores sempre pertencem a um modulo.

# Providers

Os providers são classes JavaScript simples que são declaradas como providers em um módulo.

*Providers são como services*

Os providers (fornecedores - de serviços em geral) são um conceito fundamental no nest.
A principal ideia é que eles podem ser injetados como um dependência, criando vários relacionamentos entre os objetos.

Os controladores devem lidar com solicitações HTTP e delegar tarefas mais complexas para os providers.

Os provider são inicializados junto com o aplicativo e destruidos ao final dele. Esse comportamento pode ser modificado.

# DTO - Data Transfer Object

Um DTO é um objeto que define como os dados serão enviados pela rede.

# Geral

Para criarmos uma nova rota precisamos criar o controlador e adicionar ele no modulo