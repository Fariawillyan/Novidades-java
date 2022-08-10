# Factory - inferencia - textblocks - switch

- O que foi incluído nas versões do Java desde a versão 9 até a versão 14
- O Factory Method of(..) para coleções
- Como substituir os tipos de variáveis pela palavra var
- A criar strings multilinhas sem burocracia com text blocks
- Como melhorar a escrita do switch expression

# Jshell

- Para realizar testes de algum recurso da linguagem, era necessário criar uma classe, um método main, escrever o recurso a ser testado, compilar e executar o programa
- Para facilitar a vida do desenvolvedor, criou-se uma plataforma interativa, onde o usuário, em um terminal, pode executar o código e receber respostas na mesma hora
- O terminal interativo é conhecido como REPL e já era comum em outras linguagens de programação

# Http_2

- A API HttpUrlConnection, que estava na plataforma desde o Java 1.1, possui alguns problemas como design e falta de documentação
- Criou-se, no Java 11, uma nova api, HTTP/2 Client, que ataca esses problemas com um conjunto de três classes: HttpClient, HttpRequest e HttpResponse
- Com pequenas alterações no código, é possível realizar requisições assíncronas, recurso que não era possível antes da nova API

# Reative Stream

- Trabalhar com fluxo padrão nem sempre é uma boa estratégia, pois dependendo do cenário, você terá problema de performance na sua aplicação
- Não devemos simplesmente criar uma nova thread a cada requisição, pois isso pode criar gargalos na aplicação de destino
- Uma alternativa é utilizar fluxos reativos, que paraleliza a operação, mas sempre analisando o back pressure
- Para ter o controle de todos os passos do fluxo, podemos implementar nossos próprios Subscribers e Processors

# JPMS - java plataform module system

- Na plataforma Java não existia uma forma elaborada de carregar JARs e classes, que foi a razão de conflitos, também chamado de classpath hell
- Para evitar esses conflitos e melhorar o encapsulamento das API's, pensou-se na modularização da plataforma
- Com o JPMS (Java Plataform Module System), é possível trabalhar com module-paths, que é a alternativa ao classpath
- Para declarar as dependências entre módulos e exportar os pacotes visíveis, é usado um arquivo chamado module-info.java