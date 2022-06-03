**ls** -- listar
**ctrl+l **-- limpar
**ls -a** -- mostra arquivos ocultos


<!--no computador, na pasta onde deseja criar o repositório, clicar com o botão direito e selecionar 'Git Bash Here' / isso vai abrir o bash já na dentro da pasta selecionada no computador-->

**git init **<!-- inicia um novo repositório / cria um novo repositório dentro de uma pasta-->
$ git init <!--enter-->

**Configurar e-mail e user name -"autor" do commit:**

$ git config --global user.email "(email do usuario"
<!--dar enter-->
$ git config --global user.name (nome/apelido)
<!--dar enter-->

$ git status <!--enter--><!--verifica o status do repositório(se teve ou não alterações)-->

**git add** <!-- mover arquivos e começar a dar inicio ao versionamento / incluir(adicionar) arquivos no repositório-->
<!--adicionando arquivo ao repositório-->
$ git add * <!--enter--><!--adiciona tudo o que está no reposítório e foi alterado-->
$ git add (nome do arquivo ou pasta) <!--adiciona somente o item descrito-->

**git commit **<!-- cria commit-->
<!-- salvando as alterações / commit-->
$ git commit -m "string" <!-- a string é a descrição do commit realizado/texto que cria a hash ou shar do commit-->

**mv**<!--move um arquivo-->
$ mv (nome do arquivo) ./(nome do outro repositório/pasta) /
<!--exemplo-->
$ mv strogonoff.md ./receitas/

$ echo > (nome do arquivo) <!--cria um novo arquivo-->

**mkdir **<!-- cria nova pasta-->
$ mkdir (nome da pasta) <!--criar nova pasta-->

$ git config --list <!--retorna a lista de todas as configurações que estão no git--> <!--Para sair da lista de confirgurações, clicar na letra 'q'-->

<!--Para alterar ou excluir uma configuração, comandos-->
$ git config --global --unset (configuração a ser alterada/deletada - user.name/user.email)
ex:
$ git config --global --unset user.name