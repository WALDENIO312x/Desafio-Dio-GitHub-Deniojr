O que é Git? Criado em 2005 por Linus Torvalds (Criador do Linux)., é um sistema de versionamento de código distribuído.



Benefícios:



Controle de versão

Armazenamento em nuvem

Trabalho em equipe

Possibilidade de melhorar do seu código através de contribuição por Forks

Reconhecimento



O que é o SHA1? É um algoritmo de encriptação (Secure Hash Algorithm) desenvolvido pela NSA (Agência de Segurança Nacional dos EUA).
Funciona tanto para arquivos quanto para objetos internos. Os dados encrIptados geram um conjunto de caracteres únicos de 40 dígitos que serve como identificação.



Quais são os objetos internos do Git?



Blobs

Trees

Commits



Porque o GIT é um sistema distribuído e seguro? O repositório do código fonte fica hospedado em um servidor da nuvem, por exemplo: Gihub.



Exemplo de uso: Supondo que há n pessoas alterando o código ( maintainers). A versão mais recente que está na máquina do servidor Web e a
versão que está com essas pessoas é a mesma, desse modo é distribuido e seguro.



Comandos úteis:



git config --list (Exibe as configurações do repositório local)

git status (Exibe o estado atual dos arquivos dentro do repositório Git)

git config --global --unset user.name (Remove o usuário em GIT)

git config --global --unset user.email (Remove o e-mail do usuário)



Workflow Local:



1.     git init (Inicializa um repositório do GIT dentro da pasta atual)

2.     git config –-global user.name "someone" (Seta o name no repositório GIT local)

3.     git config –-global user.email "someone@someplace.com" (Seta o email no repositório GIT local)

4.     git add* (Adiciona os arquivos untracked e unmodified para staged)

5.     git commit -m "some msg" (Comita a alteração com uma mensagem "some msg")

6.   git checkout -b newbranch (Cria uma nova Branch e navega para essa nova branch)

7.   git checkout newbranch (Navega para uma nova Branch criada)

8.   git branch –list (Lista as Branchs no repositório local)

9.   git branch -m novo-nome (Renomeia o nome da Branch Atual)

10. git branch –a (Lista as Branchs Locais e Remotas)





Comandos para Git Remoto:



git remote add origin https://github.com/Gultes/exemplo.git (Aponta o repositório local para o GitHUB)

git remote –v (Lista os repositórios remotos cadastrados)

git pull origin master (Puxa o repositório do GITHub para o repositório local)

git push origin master (Empurra o repositório local para o repositório do GITHub na master)



Obs: master/main podem variar o nome no GitHub, o nome usado nos comandos nesse caso vai ser sempre o do branch raíz!



	Erro ao criar adicionar uma pasta ou arquivo no git utilizando o comando: git add nomeDoArquivoOuPasta


Another git process seems to be running in this repository, e.g. an editor opened by 'git commit'.
Please make sure all processes are terminated then try again. If it still fails, a git process may
have crashed in this repository earlier: remove the file manually to continue.

	Acontecendo isso deve dar o seguinte comando para excluir o index que esta causando o erro no git: rm -f .git/index.lock

Depois é só preceguir utilizando o comando para adicionar o arquivo e/ou pasta
