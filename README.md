# github-study-roadmap





Este material tem por objetivo treinar a utilização e Boas Práticas de organização no GitHub, o roteiro do estudo foi criado por mim, com auxilio e "tutoria" do chatgpt, os comandos básicos do GitHub já tenho alguma familiaridade portanto, nesta etapa da atividade já realizei a criação do repositório no meu GitHub, realizei a criação da pasta de nome igual ao repositório em meu computador local, nesta pasta de repositório local inicializei utilizando o "git init", Realizado a troca de branch, inicialmente estava na branch (MASTER), então utilizei o comando "git branch -M main", Realizado adição do conteúdo dentro de README e adicionado na staging área(índice) através do "git add .", no próximo passo será realizado a inserção do comando (git commit -m "Realizado adição de conteúdo no README."), seguido de um git push -u oring main, como durante a criação do repositório web (GitHub) selecionei a opção de adicionar o arquivo readme, com essa opção marcada o meu repositório web inicial não estava vazio, isso fez com que a estrutura inicial de código do git não aparecesse, então minha pasta local ainda não está vinculada ao link do repositório remoto, portanto vou utilizar o código "git remote add origin https://github.com/VandersonCani/github-study-roadmap.git", para que a minha pasta local do github-study-roadmap fique sincronizada com a pagina web github-study-roadmap, assim consigo manter as alterações utilizando sempre os comandos básicos do git. Realizado primeira etapa de atividade de treino do GitHub.

Utilizado o comando "git log":



====================================================================================================================================================================



commit 10a7079fcbbd99d3c1469f2d91837621409d64d3 (HEAD -> main, origin/main)

Author: Vanderson Cani [vanderson.alex.cani@gmail.com](mailto:vanderson.alex.cani@gmail.com)

Date:   Tue Mar 24 09:08:37 2026 -0300



&#x20;   Realizado edição do arquivo Readme



commit 4fd986a695ccd1415b33c6c8caa28cb7aebee9ed

Author: Vanderson Cani [vanderson.alex.cani@gmail.com](mailto:vanderson.alex.cani@gmail.com)

Date:   Tue Mar 24 09:01:43 2026 -0300



&#x20;   Realizado adição de conteúdo no README.



commit b54d650d49b6c31b42e8f42ca19c73311e83849b

Author: Vanderson [164271531+VandersonCani@users.noreply.github.com](mailto:164271531+VandersonCani@users.noreply.github.com)

Date:   Tue Mar 24 08:49:36 2026 -0300



&#x20;   Initial commit



====================================================================================================================================================================



Como podemos ver os comentários a cada commit adicionado recebe um hash de identificação, no caso atual da minha evolução de trabalho o ponteiro "HEAD" está apontando para a branch main, no caso minha branch local, lembra que quando criamos o repositório local fizemos alteração da branch master para a branch main? naquela etapa criamos a branch local chamada main, e "origin/main" significa que nosso repositório web no GitHub está apontando para o mesmo commit, ou seja nessa etapa estamos com ambos sincronizados, agora vou realizar um salvar nesse documento e vou utilizar o comando "git status". 



====================================================================================================================================================================



$ git status

On branch main

Your branch is up to date with 'origin/main'.



Changes not staged for commit:

&#x20; (use "git add <file>..." to update what will be committed)

&#x20; (use "git restore <file>..." to discard changes in working directory)

&#x20;       modified:   README.md



no changes added to commit (use "git add" and/or "git commit -a")



====================================================================================================================================================================

O retorno do git status nos mostra que temos alterações não preparadas para o commit, o retorno do git status nos mostra também que temos alterações que precisam ser adicionadas utilizando o comando "git add .", e depois utilizar o comando (git commit -m ""), curiosidade, como boa prática de utilização do git é interessante realizar adições separadas, o comando "git add ." realiza adição de todos arquivos que foram alterados dentro do repositório e o commit subsequente vai aparecer em todos os arquivos modificados, isso gera ruido de informação pois dependendo da quantidade de arquivos modificados e adicionados no dia, o comentário seria muito extenso para poder abordar todas modificações, sem contar que não seria nada organizado, então para treinar essa boa prática de adição estarei realizando a criação de um novo arquivo chamado "texto\_de\_teste.txt". esse arquivo vai ser criado enquanto ainda não adicionei essas alterações que estarão selecionadas entre =====.

====================================================================================================================================================================

Arquivo salvo. 



Nessa etapa estamos com o arquivo editado, mas não adicionado nem commitado. 



Criado novo arquivo no repositório local chamado "texto\_de\_teste.txt".

Executado novamente o comando git status após a criação do arquivo, no console podemos ver que agora temos informações sobre um arquivo que foi modificado, e um arquivo que foi adicionado.



====================================================================================================================================================================



$ git status

On branch main

Your branch is up to date with 'origin/main'.



Changes not staged for commit:

&#x20; (use "git add <file>..." to update what will be committed)

&#x20; (use "git restore <file>..." to discard changes in working directory)

&#x20;       modified:   README.md



Untracked files:

&#x20; (use "git add <file>..." to include in what will be committed)

&#x20;       texto\_de\_teste.txt



no changes added to commit (use "git add" and/or "git commit -a")



====================================================================================================================================================================



agora vamos adicionar um arquivo por vez comentando separadamente, assim nosso repositório vai ficar devidamente comentado conforme as alterações vão sendo feitas.

vou utilizar o comando "git add texto\_de\_teste.txt"



====================================================================================================================================================================



XXXXXXXXXXXXXXXX \~/Desktop/Faculdade/github-study-roadmap (main)

$ git add texto\_de\_teste.txt



XXXXXXXXXXXXXXXX \~/Desktop/Faculdade/github-study-roadmap (main)

$ git status

On branch main

Your branch is up to date with 'origin/main'.



Changes to be committed:

&#x20; (use "git restore --staged <file>..." to unstage)

&#x20;       new file:   texto\_de\_teste.txt



Changes not staged for commit:

&#x20; (use "git add <file>..." to update what will be committed)

&#x20; (use "git restore <file>..." to discard changes in working directory)

&#x20;       modified:   README.md



====================================================================================================================================================================



Como podemos ver, agora nosso arquivo novo que antes não estava no estagio de commit, está aguardando o comentário sobre as alterações desse arquivo, enquanto nosso arquivo README que está sendo modificado ainda atualmente não foi adicionado portanto não será "commitado", vou utilizar o comando (git commit -m "arquivo adicionado chamado texto de teste, nele contém mais informações sobre sua utilidade e funcionalidade"). logo após utilizarei o comando git status e adicionarei a resposta do console abaixo. 



====================================================================================================================================================================



XXXXXXXXXXXXXXXX \~/Desktop/Faculdade/github-study-roadmap (main)

$ git commit -m "arquivo adicionado chamado texto de teste, nele contém mais informações sobre sua utilidade e funcionalidade"

\[main 4fd0811] arquivo adicionado chamado texto de teste, nele contém mais informações sobre sua utilidade e funcionalidade

&#x20;1 file changed, 1 insertion(+)

&#x20;create mode 100644 texto\_de\_teste.txt



XXXXXXXXXXXXXXXX \~/Desktop/Faculdade/github-study-roadmap (main)

$ git status

On branch main

Your branch is ahead of 'origin/main' by 1 commit.

&#x20; (use "git push" to publish your local commits)



Changes not staged for commit:

&#x20; (use "git add <file>..." to update what will be committed)

&#x20; (use "git restore <file>..." to discard changes in working directory)

&#x20;       modified:   README.md



no changes added to commit (use "git add" and/or "git commit -a")



====================================================================================================================================================================



Como podemos ver após o commit sobre a adição do texto\_de\_teste.txt, apenas o arquivo modificado se mantém na lista do git status com pendencia de commit, agora como ele é o ultimo arquivo a ser modificado, vou utilizar o comando "git add README.md",e depois vou comentar utilizando (git commit -m "Terminado atividade sobre utilização dos comandos git status, log, add"), após a utilização desses dois comandos vou adicionar aqui em baixo o resultado dos comandos git status e git log, para analisarmos o comportamento do git após todos arquivos e comentários estarem devidamente atualizados. 

