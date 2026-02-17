	# Changelog - Backup script
	
	## [2.0.0] - 17/02/2026
	**BREAKING**
	- Alterado layout do last_bkp.txt
	### Added
	- Criado o parâmetro 'd' para backups de domingo.
	- Implementada interface gum.
	- Implementado compactação e criptografia com | (pipe), assim é gerado um arquivo único, reduzindo I/O.
	- Implementada limpeza do diretório de backups no domingo.
	- Implementada cópia do arquivo
	### Changed
	- Funcionalidades separadas por funções.
	### Removed
	- Logs e todas as funções relacionadas foram removidos.
	- Saídas dos comandos não são mais exibidas na tela.
	- Cópia do last_bkp.txt não será mais realizada.
	
	## [1.5.0] - 08/02/2026 (44be131)
	### Added
	- Implementada cópia do arquivo last_bkp.txt
	
	## [1.4.1] - 02/11/2025 (9d488fd)
	### Fixed
	- Corrigido bug que fazia não encontrar o arquivo last_bkp.txt
	
	## [1.4.0] - 22	/10/2025 (fa6cfbf)
	### Changed
	- No backup p, criada opção para voltar, algo necessário para que a TARDIS funcione melhor.
	
	## [1.3.0] - 19/10/2025 (1c04e03)
	### Added
    - Criado o arquivo last_bkp.txt, que serve como whitelist e controle de datas de backups. 
    ### Changed
    - O backup ts passa a validar se a data de alteração do diretório é posterior à data do último backup, antes de realizar.
    
    ## [1.2.1] - 28/09/2025 (c1b1691)
    ### Added
    - Agora o script valida se o parâmetro informado é válido.
    - Criada remoção do arquivo de log dos backups t e ts.
    ### Changed
    - Criada function para compactação, criptografia e remoção dos arquivos. 
    
    ## [1.2.0] - 26/09/2025 (f0159be)
    ### Fixed
    - Caso fosse informado o mesmo diretório 2 vezes, ele fazia o mesmo backup, agora ignora a segunda vez.
    ### Added
    - Implementação realizada para permitir selecionar mais de 1 diretório no backup parcial.

    ## [1.1.0] - 24/09/2025 (49cf7f3)
    ### Fixed
    - Validação de parâmetros ao chamar o backup
    - Trata diretórios com espaços como um só.
    ### Added
    - Implementada geração de log
    - Implementada criptografia de log e remoção do arquivo original
    - É criado um log para cada diretório
    ### Changed
    - Caminhos de diretórios colocados em variáveis
    
    ## [1.0.0] - 27/09/2025 (7d881ab) 

