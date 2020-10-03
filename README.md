Como Criar/Configurar/Verificar um repositório


    
  Um repositório é o maior bem de qualquer projeto controlado por versão. Para transformar qualquer diretório em um repositório GIT, o simples comando:
 git init <directory> pode ser utilizado. Uma pasta chamada .git também deve começar a existir no diretório em que o comando foi executado. *

  Por outro lado, se você já tem um diretório e deseja verificar (clone-lo), você pode usar o comando git clone. Se você estiver tentando verificar um repositório local, use o seguinte comando:
    git clone /path/to/local/repository *

Se você pretende verificar um repositório armazenado remotamente, use: 
    git clone user.name@host:/path/to/remote/repository *

  Se você tem uma conta na Hostinger, você pode facilmente clonar e gerenciar repositórios via Painel de Controle > GIT. Por exemplo, se você quer clonar um repositório GIT, basta digitar seu endereço, escolher um ramo e instalar o caminho, e clicar no botão criar.



