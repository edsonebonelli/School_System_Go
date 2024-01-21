# Integração Contínua e Entrega Contínua 

# Tecnologia Usada
> - [x] HTML5.
> - [x] CSS3.
> - [x] GO
> - [x] Container Docker
> - [x] Pipeline
> - [x] GitHub
> - [x] GitHub Actions
> - [x] InteliiJ

# Etapas da Branch Pipeline e Github Actions

# Conhecendo o CI
> - Ver o que será necessário para executar a aplicação, sendo que no nosso caso é necessário o Docker e o Go, sendo o Docker para o nosso banco de dados e o Go para gerir a aplicação.
> - Subir o banco de dados da aplicação através do docker compose, e automatizar assim parte da tarefa, ao invés de ter que lembrar e executar o comando padrão do Docker.
> - Corrigir um problema que se encontrava no docker compose, que estava com complicações nos volumes, onde os arquivos são armazenados, permitindo assim que o banco de dados possa ser executado.

# Testando a Aplicação
> - Executar os testes automatizados para o Go, e por meio disso verificar se existem problemas de lógica na aplicação, para que sejam corrigidos.
> - Executar os testes de forma verbosa, para que assim seja possível ver todos os testes que estão sendo executados e como estão sendo executados. Assim podemos ver se algum deles retornou um erro.
> - Acessar o Github Actions, para que possamos começar a criar as rotinas de integração contínua.
> - Criar a sua primeira rotina de CI, utilizando a rotina sugerida pelo Actions, e assim permitir que apenas poucas linhas sejam alteradas.

# Customizando a Rotina
> - Quais são os principais campos dos jobs, tendo o runs-on para escolher o sistema, steps em conjunto com run para executar códigos e name para nomear cada passo.
> - Como executar códigos dentro da rotina de CI, para que assim possamos preparar o ambiente e rodar os testes da aplicação, garantindo a lógica dela.
> - Iniciar um container Docker usando o docker-compose up dentro de uma pipeline, e com isso conseguimos facilitar a configuração do ambiente.

# Segunda Rotina
> - Alterar a ordem de execução de comandos dentro de cada job, tornando-os mais rápidos, como no caso dos testes e a compilação, nos quais não é necessário gastar tempo com a compilação se os testes falharem.
> - Criar um segundo job, o que permite o separar melhor cada função dentro da rotina, facilitando a identificação de problemas e a manutenção a longo prazo.
> - Visualizar as rotinas no Github Actions, e verificar se ocorreu algum erro e acessar os logs de execução.
> - Forçar um erro, podendo assim entender o que ocorre se for encontrado isso na aplicação e como esse erro é mostrado para que acessa o repositório.

# Utilizando estratégias
> - Trabalhar com estratégias de matrizes, o que possibilita a criação de vários ambientes de desenvolvimento diferentes com pouco código, deixando a rotina mais organizada.
> - Criar e utilizar variáveis, como a go_version dentro da estratégia de matriz,o que possibilita guardar múltiplos valores para usarmos posteriormente.
> - Utilizar o secrets, e criar assim um ambiente, colocando um segredo dentro dele, possibilitando o seu uso dentro da rotina, porém sem compartilhar seu valor.
