**SSH**- No git Bash: 
<!--comandos para gerar a chave: -->
$ ssh-keygen -t ed25519 -C (email do usuario github) 
<!--dar enter-><!--vai mostrar a informação de que está genrando a chave e o local onde será armazanada a chave --><!--dar enter--><!--cadastrar senha--><!--chave criada, vai mostar onde as chaves publica e privada foram criadas-->

<!--entrar na pasta .ssh *** comandos: -->
cd C/Users/(usuário)/.ssh

<!--comando para visualizar a chave pública-->
$ cat id_ed25519.pub
<!--vai aparecer a chave *** copiar a chave e colar no GitHub-->

<!inicializar o ssh agent--><!--dentro da pasta .ssh, comandos-->
$ eval $(ssh-agent -s)
<!--dar enter--><!--vai aparecer o numero de star do processo-->

<!--entregar a chave privada para o 'agent' controlar--><!--dentro da pasta .ssh, comandos-->
$ ssh-add id_ed25519
<!--dar enter--><!--colocar a senha cadastrada na criação das chaves--><!--vai aparecer a mensagem confirmando que a identidade foi adicionara-->

<!--ao usar a chave com o GitHub pela primeira vez, vai aparecer uma mensagem de autenticidade. Basta selecionar sim, para salvar a assinatura-->

 