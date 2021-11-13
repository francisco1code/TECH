<center>

# Bem vindo!

</center>

Nesse documento será listas todas as tarefas realizadas. Foram definido algumas [issues](https://github.com/francisco1code/Desafio-Tech-DevOps/issues) onde temos algumas taks, e em cima dessas issues foram desenvolvidas as "feature", e a maioria dos commit tem um link direto para issue.

<center>

## Entrega Obrigatoria

</center>

### [Docker](https://github.com/francisco1code/Desafio-Tech-DevOps/blob/main/prod/Dockerfile) e [Docker-compose](https://github.com/francisco1code/Desafio-Tech-DevOps/blob/main/docker-compose.yml)

**Docker**: O docker foi usado para containizar a aplicação feita em react. Nesse caso  o dockerfile para criar uma imagem da nossa aplicação e em react.
**Docker-compose**: Esse é um dos Orquestradores de contêineres, que na prática ajudar na administração dos contêineres, na nossa aplicação ele está criando os contêineres a parti da imagem que criamos no dockerfile, e foi iniciando o Nginx a partir de uma imagem pronta e também está sendo feito a bind de portas do container com sua máquina local, com isso a aplicação estará rodando no container na porta 3000, e no seu localhost na porta 3333, além disso estamos configurando volumes e network.

<center>

##  Entregas Extras

</center>

### [Nginx](https://github.com/francisco1code/Desafio-Tech-DevOps/blob/main/nginx/nginx.conf)

Estamos utilizando o Nginx na nossa aplicação com função de proxy reverso, além disso podemos usar o Nginx como memória cache, balanceador de carga etc. Na aplicação está sendo feito um redirecionamento da porta 80 -> 3000, assim quando acessamos a porta 80 conseguimos acessar nossa aplicação perfeitamente.

### [Pipeline CI](https://github.com/francisco1code/Desafio-Tech-DevOps/runs/4196778233?check_suite_focus=true)

Foi criando uma **pipeline CI** bem simples com github action, essa pipeline faz um build geral da aplicação quando você abrir um **PR** ou **PUSH** direto para master (Detalhe o github foi configurado para não aceita push direto na master, apenas por **PRs** para assim tem o maior controle dos commits), caso o build passe sem quebrar vai ser possível fazer o merge.









