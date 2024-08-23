# avaliacao-jp

Comandos Git
 
git clone <'URL do repositorio'> .. Ele clona um repositorio remoto em sua maquina local com os links

git branch -d <'nome da branch'> .. Ele deleta a branch com o nome que voce colocou (apenas da sua maquina local)

git init .. Ele cria um repositorio em sua maquina local e é melhor fazer em pastas para deixar mais organizado

git fetch .. Ele serve para para sincronizar o seu repositorio local com o remoto (as informaçoes vindo do remoto atualiza as do local)

git push .. Ele manda as informaçoes que foram alteradas, criadas, deletadas para o repositorio remoto 

git checkout -b <'nome da branch'> ..Ele cria uma branch nova e automaticamente voce entra nessa branch

git branch ..Ele ira mostrar todas as branch locais que tem

git branch -r ..Ele ira mostrar todas as branch remotas que tem

git branch -a ..Ele ira mostrar todas as branch locais e remotas que tem

git status .. Ele serva para voce ver todos os arquivos que foram alterados, arquivos novos e tambem arquivos que estao prontos para commit

git pull .. ele tras a informaçoes do repositorio remoto para a branch usada no momento (use git reset --hard <'commit-hash'> ele muda a branch para o commit que tinha antes do pull)

git merge <'nome da branch'> .. Ele da um merge(mescla) a branch que voce esta na branch que vc solicitou

git checkout <'nome da branch'> .. Ele serve para voce mudar de branch colocando o nome da branch

git add <'nome do arquivo ou .> .. o (.) serve para selecionar todas os arquivos e colocar na staging area e apenas o nome do arquivo coloca so ele na staging area para fazer o proximo commit (use git rm --cached <'file'> para tirar os arquivos da staging area)

git commit -m "<'descriçao'>" faz o commit com uma mensagem (use git reset --soft HEAD~1 para desfazer o ultimo commit mantenda as mudanças no arquivo ou git reset --hard HEAD~~1 para tirar o commit e as mudanças)

comandos git de configuração

git --version .. para ver a versão do gir

git config --global user.name "seu nome" .. configura seu nome do github no git local

git config --global user.email "seu email" .. configura seu email do github no git local

SSH

ls -al~/.ssh .. para ver se tem alguma ssh ativa

ssh-keygen -t ed25519 -C "seu email" .. Adicona uma chave ssh

eval "$(ssh-agent -s)" .. inicia um agente pata colocar sua  chave ssh

ssh-add ~/.ssh/id_ed25519 .. adicona a chave ssh ao agente

clip < ~/.ssh/id_ed25519.pub .. copia a chave ssh 

ssh -T git@github.com ..testa para ver se sua chave ssh esta funcionado se funcionar digite yes e de enter