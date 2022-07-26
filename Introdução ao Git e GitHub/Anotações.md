**Link para download do Git:** https://git-scm.com/downloads

# GIT

Software de **versionamento** de código - cria e monitora versões diferentes do código.

*Vantagens:*

* controle de versão
* armazenamento em nuvem
* trabalho em equipe - colabração
* melhorar o código
* reconhecimento - portfólio



*Como o Git funciona?*

**SHA1** Secure Hash Algorithm - conjunto de funções criptográficas projetadas pela NSA - algoritmo de encriptação

que gera um conjunto de caracteres identificador de 40 dígitos, cada conjunto é único 

* identifica arquivos de forma rápida e segura
* forma curta de representar um arquivo



​		**SISTEMA**

​				**DISTRIBUÍDO** contribuições diferentes a um mesmo código (diferentes autores)

​				**SEGURO** a criptografia SHA garante a rastreabilidade de todas as infos, pois cada objeto tem seu próprio SHA



*Objetos internos fundamentais do Git*

* Blobs
  * tipo do objeto
  * tamanho da string ou do arquivo
  * conteúdo do arquivo
  * armazena os metadados do Git
  * \0
* Trees
  * armazena os blobs
  * também contém metadados
  * armazena o nome do arquivo
  * onde estão os arquivos ("pastas")
* Commits
  * contém informações sobre
    * tree
    * parente (último commit realizado antes desse)
    * autor
    * mensagem (flag: -m) - explica o que foi commitado, as atualizações nos arquivos
    * timestamp
    * também tem criptografia SHA



*Ciclo de vida dos arquivos dentro do Git*

- git init: inicializa um repositório
- git add: adiciona arquivo para estado "Staged"
- git commit: adicionar as atualizações mais recentes
- git push: empurrar o commit para o repositório (GitHub)
- git pull: baixar arquivo do repositório para a máquina (usado para resolver ***merge conflicts***, por ex.)
- git config: mostra as configurações - verificar user.name e user.email, deve ser o mesmo do cadastro do repositório (GitHub) para não ocorrer erro de compatibilidade
- git config --global --unset user.name (por ex.): reseta a configuração
- git config --global --set user.name: adiciona a configuração
- git clone URL: clona o repositório do diretório (GitHub) para a máquina



# GITHUB

Repositório remoto/online para armazenamento de códigos

*Cadastrar* - atenção ao e-mail e user.name, que preferencialmente devem ser os mesmos usados no Git



*Autenticação* - em ago/21 houve uma atualização no modo de enviar os códigos do Git para o Git Hub, tornando tudo mais seguro.



**CHAVE SSH** forma de estabelecer uma conexão segura e encriptada entre duas máquinas

Servidor do Git Hub <----conexão----> minha máquina: configurada como uma máquina confiável, o Git Hub já vai reconhecer a "assinatura" da minha máquina



***Git Bash*** terminal extendido para otimizar o uso do Git (ambiente de comandos)