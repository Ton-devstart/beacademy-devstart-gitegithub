# Git e Github

Repositório criado para os entregáveis do curso de Git e Github da beacademy-paylivre.

Professores: Régis Santos e Luan


Git - Configuração Inicial

git config --global user.name “nome_do_usuário”
git config --global user.email “email do usuário”.


Git - Repositórios

Comandos:
- git status: mostra as informações dentro do repositório.
- git init: inicializa um repositório.
- git add .: adiciona um arquivo ou alteração ao commit.
- git rm --cached <file>: desfaz a adição de um arquivo ao commit.
- git commit -m “mensagem”: cria o commit com uma mensagem relacionadas com as alterações do projeto.
- git log: histórico dos commits.

Conceitos:
- branch: 
    - são ramificações do projeto.
    - por elas posso acompanhar o desenvolvimento e incrementar soluções.
    - elas são principais e auxiliares.
    - antes de navegar entre branchs é preciso saber quais alterações estão aguardando para serem comitadas.
- untracked files: 
    - arquivos sem rastreio;
    - não podem ser versionado. 
    - eles passam a ser rastreados a partir do momento que participam de um commit.
- commit:
    - registra as alterações de um projeto.
	- é possível adicionar todos os arquivos que foram criados, alterados ou excluídos ou de forma individual.
	- possui mensagens sobre o que está sendo realizado: nova funcionalidade, correção de bug, etc.


Git - Ramificação

Comandos:
- git branch: mostra as branch locais e em qual eu estou naquele momento.
- git branch nome_da_branch: cria uma branch; para espaço posso usar hífen e anderline.
- git checkout nome_da_branch: navega de um branch para outra.
- git checkout -b nome_da_branch: cria uma branch e faz o checkout/acesso.
- git branch - d nome_da_branch: remove uma branch.
- git merge nome_da_branch: unifica as alterações das branchs.

Conceitos:
- main: nome da branch principal/master.


Github - Configuração

Configuração:
- acessar https://docs.github.com/pt/authentication/connecting-to-github-with-ssh.
- clicar em “Gerar uma nova chave SSH e adicioná-la ao ssh-agent”.
- abrir o git bash e colar ssh-keygen -t ed25519 -C "your_email@example.com".
- na pasta c/Users/nome_do_usuário/.ssh abrir o arquivo .pub com bloco de notas e copiar a chave.
- acessar https://github.com/settings/keys e clicar em “New SSH Key”.
- colocar um titulo e colar a chave.


Github - Criando Repositório

Criando:
- acessar https://github.com/Ton-devstart?tab=repositories e clicar em “New”.
- preencher o nome do repositório.
- marcar “Add a README file” para criar um branch main.
- gitignore template: identifica arquivos que não serão verificados pelo controle de versão do git.
- clicar em “create repositor”.
- ir e “Code”, copiar o endereço que está no SSH e colar no terminal git bash através do comando git clone.
- ainda no terminal, acessar o diretório criado por meio do endereço copiado que contém o nome do repositório com o comando “cd ...”

Enviar alterações:
- abrir o arquivo “REDME” no repositório local, fazer as alterações necessárias e salvá-lo.
- não é necessário enviar as alterações em cada commit, ou seja, pode-se usar o git push de uma só vez.
- após acessar o diretório criado, adicionar o arquivo (git add.), comitar (git commit -m “comentário”) e fazer push.


Versionamento de Projeto

Conceitos:
- separa/guarda um arquivo sem precisar fazer commit para resolver outras solicitações.

Comandos:
- git stash: mostra os arquivos guardados no stash.
- git stash list: volta o stash mais recente.
- git stash pop: aplica o stash mais recente.
- git stash apply: qual stash voltar.
- git stash drop: limpa o stash.
