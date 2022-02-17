# Primeiros conceitos sobre Branches



*Branches são versões ramificadas de um codigo, de uma commit, de um projeto onde você pode criar uma ramificação para trabalhar no projeto salvando em um local seguro, enquanto existe paralelamente o projeto raiz onde podem alterar e versionar o mesmo projeto, e você pode juntar sua versão com a versão do projeto raiz ou alteração do projeto raiz com o seu.*


Comandos de commit e localização do HEAD(onde você está trabalhando com a Branches)

**git commit -m “nome do arquivo”**

**git checkout -b “nova branche”** - movimenta o Head de uma Branche para outra (-b é utilizado para criar uma branch)

**git marge “nova branche”** - junta duas branche

**git config –global –unset user.email** (*para resetar o e-mail do commit*)

**git config –global –unset user.name** (*para resetar o nome do commit*)

**git config –global user.email** (*para add um novo e-mail do commit*)

**git config –global user.namel** (*para add um novo nome do commit*)

**git config –list** (*para listar o conteúdo do commit*)

**git branch** (*indica quais branchs existem em seu repositório*)

**git branch -m nomeDaBranch** (*renomeia a branch onde você está atualmente*)

**git branch -m nomeDaBranch nomeDaBranchNova** (*renomeia a branch que você quer, mesmo estando em uma branch diferente*)

**git branch -d nomeDaBranch** (*Deleta a branch que você quer*)

**git stash save “quantidade de arquivos que existirem dentro do branch e você que guardar no stash”** (*Cria um stash um tipo de caixa ou pasta que mantêm os arquivos contidos nela apenas naquela branh especifica, assim evitando que os arquivos se movam de uma branch para outra quando mudarmos de branch para trabalhar*)

**git stash list** (*Lista o stash criado para armazenar seus arquivos de trabalho*)

**git stash pop** (*Abre ou estoura a caixa onde você guardou os arquivos para voltar a trabalhar e a mover eles*)

**git stash clear** (*Apaga todas as stash colocando os arquivos de volta na branch*)

**git log** (*Carrega todos os dados de alterações feitas naquele diretório, naquela branch, todas as alterações daquele projeto.*)

**Git log pastaOuArquivo** (*Carrega os dados e alterações apenas do arquivo ou pasta dentro daquele diretório.*)

**Git log –oneline** (*Trás as alterações de commits em apenas uma única linha*)

**git reset –soft** (*Reverte o arquivo do commit para a forma anterior, antes de ser adicionado com o comando: git add *. Ao adicionar ao código HEAD, dessa forma – git reset –soft HEAD~1 – podemos reverter o ultimo commit criado e ao acrescentar mais números como ~2, ~3, ~4 …, revertemos a quantidade criada contando de do ultimo criado ao anterior e assim sucessivamente.*)

**Git reset –mixed HEAD~1** (*Volta os arquivos para os estados anteriores, excluindo o commit anterior.*)

**Git reset –hard HEAD~1** (*Reverte o último commit*)

**git revert HEAD~1** (*Reverte o commit anterior criando um novo commit com um novo heshi passando o HEAD para esse novo commit. É o comite invertido do do commit anterior.*)
