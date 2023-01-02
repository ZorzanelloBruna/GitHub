# Comandos GitHub

# Comandos básicos para um bom desempenho no terminal

- Para acessar o terminal selecionar a tecla (Windows) e digital cmg(clicar em prompt de comando).
- Ao lado de usuário digitar dir – Em seguida vai aparecer na tela todas as  pastas presentes no  diretório do Windows.
- cd é um comando que permite navegação entre as pastas.
- digitando dir novamente (mostra a base do diretório C).
- Ao digitar cd Windows(enter) e dir(enter) mostra na tela a listagem de ditrórios dentro do Windows.
- Para retroceder(voltar uma casa) digitar cd ..
- Comandos para limpar a tela - ctrl l, cls e clear.
- Para criar uma nova pasta digita-se mkdir(dentro do diretório C ou dentro da pasta que você pretende salvar essa nova pasta).
- Função del deleta arquivos dentro de uma pasta.
- Para remover o diterório(pasta) – rmdir (nome da pasta) /S Q/ e enter.

# Como funciona o Git por "por  baixo dos panos"

 SHA1 significa algoritmo de Hash seguro, é um conjunto de funções hash criptografadas projetadas pela NSA(Agência de Segurança Nacional dos EUA).
 A encriptação gera um conjunto de characteres identificador de 40 dígitos.

 **Existem 3 objetos fundamentais do Git responsáveis pelo versionamento do código.
- BLOBS - Contém metaDados do Git.
- TREES - armazenam blobs e montam a estrutura de onde está os  arquivos.
- COMMIT - da o signficado para um monte de pasta, dentro do commit estão as trees e dentro das trees estão os blobs.

 a Chave SSH é  uma forma de estabelecer uma conexão segura e encriptada entre duas máquinas.

# Comandos para seguir e gerar chaves SSH para colocar no GitHub

- Abrir Git Bash.
- Digitar ssh-keygen –t ed25519 –C (colocar seu e-mail) enter.
- colocar sua senha .... enter.
- digitar - cd/c/Users/Usuario/.ssh/ - enter
- digitar ls depois clicar (enter)
- cat id_ed(se  quiser pode apertar tab para terminar de completar ou digitar o cógico manual. OBS: passar para o GitHub sempre a chave publica
- Copia a chave  e cola no github 
---> No GitHub ir em configurações (lado direito superior da tela)
Ssh and gpg (lado esquerdo inferior)

# Gerando número do processo
- eval $(ssh-agent –s) enter
- ls enter
- ssh-add id_(número gerado)- (passa para o agente a chave privada).

# Token de acesso pessoal
  Entrar gitHub
- lado esquerdo em baixo – developer settings
- personal acess tokens
- generate new token
- copia token gerado e cola em algum lugar seguro, o código gera somente uma vez, não tem como recuperar.

# Iniciando um Git

- Abrir Git Bash
- ls  mostra as pastas contidas no C.
 Criando uma pasta
- mkdir( nome da nova  pasta)
- git init – inicia  o código – cria-se um repositório.
- para ter acesso as pastas ocultas se usa uma flag especifica – ls –a.

# Criando um repositório no GitHub

- clicar em repositório (ícone fica no centro da página na parte de cima).
- new
- preencher o nome, descrição, selecionar add a README file, deixar público( de preferência)para que o conteúdo fique exposto para as empresas e demais desenvolvedores.
- creat repository
- após inserir o material desejado é preciso copiar o link do arquivo, pode ser copiado o link de sua preferencia(clonar)
- no seu diretório entrar na pasta que deseja salvar.
- com o botão direito, selecionar Git Bash
- digitar git clone (e colar o link copiado do GitHub)

	**Após criar uma pasta adicional com outros arquivos diretamente no seu diretório, é preciso fazer a atualização no Git e no GitHub, para que entre esse novo arquivo inserido. Para isso temos os seguintes passos:
	
--- atualizar a pasta no git --
- abrir git bash
- git status
- git add . ou git add –A . (atualia a pasta com novas informações)
Para levar as informações para o GitHub
- git commit  –m “Inclusão (nome da pasta ou conteúdo incluso)” e enter
-git push origin main (manda todos commits para nuvem).
Feito isso é só entrar no github e dar um F5  para atualizar.
