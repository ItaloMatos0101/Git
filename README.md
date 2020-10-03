# Comandos no Git
> Após a instalação e configuração do Git, é necessário compreender comandos que possibilitam operar com ele como; criar
repositório, gravar alterações, ver histórico de alterações e outras funcionalidades
	- Criação de um repositório
		git init
		esse comando cria um repositório. Deve-se ir no local onde se quer inicializar o repositório e no terminal
		dar o seguinte comando: git init. O comando cria uma espécie de subpasta na pasta do trabalho atual
		essa subpasta chama-se .git, esse ponto significa que é um arquivo oculto. Para verificar se ela foi criada, 
		no terminal deve-se dar o comando "ls -a". É dentro dessa pasta(.git) que ficará o conteúdo do projeto.

	- Alterações no repositório
		para adicionar arquivos ao repositório são usados os comandos; git add nome_do_arq e git commit -m""
		O git add adiciona arquivos que serão utilizados num futuro commit e a instrução git commit -m"" gravas
		as mudanças adicionadas pelo git add no repositório. O -m"" serve para associar um comentário ao 
		commit que esta sendo feito.
	
		git status
			esse comando é responsável por retornar o estado atual dos arquivos do diretório, em qual branch
			o programador está, os commits feitos e etc.

		git diff
			retorna mudanças feitas em arquivos já 'commitados' do diretório. Além disso, existe uma variação dessa 
			instrução que é; git diff nome_do_arq, ela retorna apenas as mudanças feitas em um arquivo específico
		
		git rm nome_do_arq
			esse comando remove arquivos do diretório.

