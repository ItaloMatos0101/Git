### - Histórico:


Para verificar o histórico dos commits efetuados em determinado repositório, existe o comando:

                                             *git log*

Esse comando mostra os commits efetuados de cima para baixo sendo o superior o mais recente. Um conjunto de informações do commit também são apresentadas como nome do autor, e-mail, data e a mensagem do commit. Existem também algumas diretivas úteis que facilitam na hora de averiguar o histórico dos commits. A diretiva -p mostra, além do histórico básico do commit, asmodificações realizadas nos arquivos.

A diretiva --stat mostra um conjunto de estatísticas úteis de cada commit, como por exemplo a quantidade de arquivos modificados e a quantidade de linhas modificadas.

### - Desfazendo:
          
Quando se é necessário desfazer alguma modificação que gerou um erro no projeto. Para poder refazer o último commit efetuado, é utilizada a diretiva --amend do comando git commit como no exemplo a seguir:
                                                  
                                               *git commit --amend*

Esse comando irá abrir o mesmo editor de mensagens de commit usado pelo sistema e, caso não tenha sido efetuada nenhuma mudança nos arquivos desde o último commit, o git irá apenas reescrever a mensagem do commit.

Caso o gerente do arquivo tenha esquecido de efetuar alguma modificação antes de realizar o commit, ele pode realizar a modificação do arquivo, entrar com o comando do gitadd recebendo como parâmetro o arquivo modificado e, refazer o commit com a diretiva --amend.

### - Repositórios Remotos:
 
Um repositório remoto do Git normalmente é hospedado da internet para que fique de fácil acesso para várias pessoas envolvidas em um projeto.

Quando você deseja compartilhar um diretório Git com outras pessoas, é necessário que você aprenda a gerenciar um repositório remoto do Git. 
Alguns dos conhecimentos necessários para conseguir gerir um repositório remoto são: adicionar um repositório remoto, remover repositórios remotos inválidos, gerenciar ramificações.

Para exibir os remotos do seu repositório. é necessário entrar com o comando:
 
                                           *git remote*

É possível ainda, utilizar a diretiva “-v” para mostrar a url completa do seu remoto.Para adicionar remotos, usa-se o comando “git remote add” 
                                          
                                          *git remote add “apelido/nome curto” “url”*

Concedendo um apelido para um remoto, quando for necessário, é possível trazer ao repositório Git apenas os arquivos daquele remoto, usando o comando “fetch” seguido apenas do apelido do remoto.
                                    
                                        *git fetch “apelido”*

É importante lembrar que o comando fetch apenas traz ao repositório os arquivos solicitados, o merge com os arquivos atuais deve ser feito de forma manual, quando o mesmo estiver pronto. Caso seja de interesse do usuário, pode-se usar o comando “pull” para trazer os arquivos, pois o mesmo já efetua merges automaticamente.

                                       *git pull “apelido”*

Quando o seu trabalho está pronto e já lhe é de interesse enviar os arquivos modificados ao remoto do projeto, usa-se o comando “push” para efetuar a tarefa. É possível enviar o arquivo para o remoto de origem ou para um remoto em específico.

                                      *git push origin master* 

Vale lembrar que, para poder escrever arquivos no repositório remoto, você necessita ter permissão de escrita.
Quando quiser ter informações sobre um remoto:

                              *git remote show “nome remoto”*

Para renomear um remoto:
                              
                             *git remote rename “nome antigo” “nome novo”*

Para remover um remoto:

                              *git remote rm “nome remoto”*
