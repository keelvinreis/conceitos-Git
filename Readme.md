# Conceitos do Git

### Olá meu nome é Kelvin e esse simples Arquivo/Projeto dos meus estudos sobre Git.

* [O que é Git;](#oque)
* [Sua Vantagem;  ](#vantagens )
* [Sua importancia no mundo do Desenvolvimento;](#importancia)
* [Como que o Git funciona;](#funciona)
* [Passo a passo/Comandos Iniciais;](#passoapasso)
* [O que é Branch;](#oquebranch)
* [Como ver o commit e sua versão;](#commitversao)
* [O que é Head;](#head)
* [Rastremento de mudanças;](#rastrear)





## <a href="#oque" style="color:white">O que é Git :</a>
 **Git é um sitemas de controle de versões.**

Esse controle de versões registra as mudanças que ocorrem no código-fonte de um projeto, o Git mantém registro de todas as modificações no código em um tipo especial de banco de dados.

Logo permite que um codigo a ser desenvolvido ou atualizado, sejam alterados de forma simultânea, por inúmeras pessoas(equipe responsável), sem ter a preocupação que essas alterações sejam sobrescritas umas pelas outras.

 ## <a href="#vantagens" style="color:white">Vantagens do Git:</a>

1. A sua **arquitetura descentralizada** é o que faz com que o Git seja diferenciado, o Git ele é distribuito o que nos permite trabalhar com ele de maneira offline com o repositorio localmente  na maquina do desenvolvedor tendo todas as versões do codigo e com isso fazer todas as alterações e quando terminarmos podemos empurrar(dar o Push) e enviar para o servidor remoto.
<img src="https://wac-cdn.atlassian.com/dam/jcr:9d51f0ee-5946-4be2-886c-ff040ef8c1a1/03.svg?cdnVersion=309">

2. Um **histórico de alterações** completo e a longo prazo de todos os arquivos.

3. **Economia de tempo** quando queremos criar uma nova funcionalidade ou voltar com alguma função basta abrir o repositorio e pegar a versão;

4. Ramificações de recursos, a ramificação fornecem um ambiente isolado para cada alteração, podendo deixar o codigo de qualidade de produção na ramificação principal, trazendo consigo a organização do que é cada ramificação/alteração.
 

 ## <a href="#importancia" style="color:white">Qual a importância do Git:</a>

A importancia do Git é muito grande, quando se tem +1 pessoa para se trabalhar no desenvolvimento de um codigo se utiliza o Git fazendo uma nova versão do codigo acada acrecimo de linhas deixando atualizado com um novo versionamento e caso ocorra algo inesperado é facil de voltar a versão do codigo para uma antecessora essa é a grande importancia quando quisermos criar algo em time ou corrigir algo sem ter que fazer tudo novamente. 

## <a href="#funciona" style="color:white">Como que o Git funciona:</a>

Git trabalha em uma arquitetura em Branch (ramificações). 
Cada novo commit, ou seja, alteração do código, cria um novo ponto na historia/ramificação atual (uma branch).

<img src="https://wac-cdn.atlassian.com/dam/jcr:a905ddfd-973a-452a-a4ae-f1dd65430027/01%20Git%20branch.svg?cdnVersion=309">



## <a href="#oquebranch" style="color:white">O Que é Branch:</a>
<p align="center">
O Git trabalha como se fosse uma linha do tempo e esta linha seria o nosso branch principal, que é conhecido como master.
</p>

**Branch Significa** Ramo e quando criamos um repositorio ja se cria o ramo principal "Master ou Main".

**Master:** é o ramo principal um ramo de produção, onde eu tenho uma versão do meu software/codigo que esta sempre sendo ultilizado.

**O intuito da Branch criada:** Nos bastidores enquanto o software/app é usado, desenvolvemos a nova versão, e é ai que criamos um branch saindo da master erdando todo o funcionamento para que corrijamos ou criamos novas funcionalidade.

<p align="center">
  <img src="https://sonassets.s3.amazonaws.com/transcricoes/git-e-github/feature-branch.png" width="600" height="300" >
</p>

 

## <a href="#passoapasso" style="color:white">O passo a passo:</a>
* O Git cria um repositorio local no diretorio do Projeto;
* Esse repositorio local pode ser clonado para um rpositorio remoto;
* E um remoto pode ser criado e clonado para um local.

         1º Criamos uma pasta para o projeto que vamos desenvolver.
         2º Botão direito e gitBash. 
         3º Digitar Git init onde ira criar um repositorio local.
         4º Houve uma criação da pasta .Git (uma pasta oculta).
         5º A pasta oculta é onde ira armazenar o Projeto a ser desenvolvido.
         6º Em .Git existe a pasta 'object' ela é a responsavel pelo grafo de commits.

         7º Antes de armazenar no repositorio e formar o Grafo... o git precisa genrenciar o projeto.

         Grafo de commits: onde o git representa as mudanças atraves de um grafo com os commits os comentario.
#### Exemplo:       
<img src="https://live.staticflickr.com/65535/52004212571_2ebf4c9100_c.jpg" width="500" height="500">


            7.1 Em seu estagio inicial para colocarmos o arquivo/nova versao precissamos dar `['Git add']`
            7.2 O Git add coloca na area de staging(preparação) onde é adicionado todos os arquivos e pastas que foram criados ou modificadas.
            7.3 O `['git status']` mostra o que tem dentro dessa area.
            7.3 O `['Git commit']` identifica e armazena o "container" no repositorio `[.Git]`
            e dentro desse repositorio os "containers" precisam ser identificado.
#### Exemplo:

<img src="https://live.staticflickr.com/65535/52004570341_498cacf118_b.jpg" width="500" height="500" alt=".GIT">

#### Descrição:
 _Quando o Git executa o comando `[Git commit -m]` acontece o **envio para o repositorio**, logo após o **Git versiona o projeto** em um ponto, esse ponto é o inicio do que chamamos de Ramificação que consequentemente cria o "Grafo de commits, vamos ver com mais detalhe no assunto a seguir._

## <a href="#commitversao" style="color:white">Como vemos cada commit e versão:</a>

Usando o comando fornecido pelo Git o `[Git log]` nos permite identificar de maneira extensa, quem alterou e qual o Id/hash do commit e a sua mensagem. 
#### Exemplo:
<img src="https://live.staticflickr.com/65535/52006183834_0d5c67144b_b.jpg" width="600" height="100" alt="exemploGitLog">

Usando o comando `[Git log --oneline]` vizualizamos o commit atual que esta selecionado e nos permite ver o Hash do commit e a mensagem. 
* **Detalhe:** a Hash vem com os 7 primeiros caracteres.
#### Exemplo:
<img src="https://live.staticflickr.com/65535/52006488110_53f3f0c0cb_b.jpg" width="600" height="100" alt="gitOneline">

### <a href="#head" style="color:white">O que é o Head:</a>
No codigo vemos `(HEAD -> Master ou Main)`. O head é uma especie de ponteiro. Mostra onde o nosso projeto se encontra no grafo de comits e a ramificação, vamos entrar no https://git-school.github.io/visualizing-git/ e ver com detalhes.

Perceba que o Head acompanha cada commit realizado assim como tambem mostra a ramificação padrão, ele sempre acompanha o ultimo commit feito.

<img src="https://live.staticflickr.com/65535/52006130593_85a6da6035_z.jpg" width="500" height="500" alt="HEAD">

### Analogia importante: 
O Git não gera copias do projeto a cada Commit, isso traria perda de performace. O git abre "Abre o Container" acresenta alteração feita e depois da um novo Hash identificação para poder identificar a nova versão. O HEAD acompanha o processo.


<img src="https://live.staticflickr.com/65535/52006374329_5ca0281f4f_z.jpg" width="437" height="640" alt="gitHead">

## <a href="#rastrear" style="color:white">Rastrear mudanças e recuperar versões:</a> 
*Se com o Head podemos selecionar cada commit "container" que armazena a versão e tem seu propio Hash, então podemos recupera-lo caso precisamos.*

*Usando o `[Git Checkout 'hash do commit']` - o arquivo volta a versão anterior.*

<img src="https://live.staticflickr.com/65535/52006199108_3b3bc61fb2_z.jpg" width="500" height="500" alt="gitcheck">

*Usando o `[Git log --oneline ]` - o git só mostrara os commits anteriores .*

*Usando o`[Git Branch ]` - o git nos mostra para qual commit o head esta apntando .*

*Usando o `[Git checkou master ]` - o git retorna para versão atual.*

<img src="https://live.staticflickr.com/65535/52006440954_64954451bc_z.jpg" width="640" height="292" alt="Anotação 2022-04-15 111817">

*1º Comando: Git init*

->  Cria um repositorio vazio(Uma pasta que iremos armazenar o nosso codigo) & cria uma breanch (Master) 'linha do tempo de versões principais em uma linha coronologica'.

Tecnica e conhecimento: Uma boa pratica é criar uma nova ramificação, se por exemplo estivermos um Software grande e acada alteraçao que formos fazer for ficar na "Master" seria diversas versões, então para uma melhor pratica criar ramificação e atualizar a master logo ter terminado a alteração e proporcionando um bom controle de versão é uma otima pratica.

*2º Comando: Git add arquivo ou . caso seja todos*

-> Adiciona na area de staging(staging area permite que seja realizado vários commits a partir dela).
 Uma area que o arquivo ira ficar aguardando o commit e O comando git add mantém o histórico de todas as ações realizadas no código, permitindo que, se algum problema ocorrer na aplicação, o comando de desfazer alteração possa ser acionado. 

*3º Comando: Git status*

-> Mostra se tem atualizaçoes feita no arquivo que devem ser comitadas afim de criar uma versão.

*4º Comando: Git -m commit "mensagem para informação do que foi alterado"*

-> Salva a nova versao do seu arquivo.

*Conexão para o Git-Hub*

*5º Comando: Git remote add origin https://github.com/nomeUsuario/pastaRepositorioLocal.git*

-> Estabelecimento de onexão com o repositorio local para o repositorio online gitHub.

*6º Comando: Git push -u origin master*

-> Coloca a nossa ramificação principal no repositorio.

*Fazendo uma nova versão atualizando o arquivo*

*1º Comando: Git add .*

-> Seleciona esse arquivo e o move para a área de teste, marcando-o para inclusão no próximo commit.

*2º Comando: Git status*

-> Informa se tem alguma alteração.

*3º Comando: Git commit -m "mensagem para informação do que foi alterado"*

-> Alteração salva no repositorio da maquina.

*4º Comando: Git push origin master*

-> Alteração enviada para o GitHub.

**Criação de de Branch: Uma ramificação do projeto**

-> Normalmente se cria uma Branch para uma criação de uma Feature, adicionar uma pagina no projeto, um botão...

*1º Comando: Git checkout -b "Nome da Branch"*

->criação de uma nova Branch saindo da linha cronologica principal (Master).

*2º Comando: Git add .*

*3º Comando: Git commit -m "mensagem"*

*4º Comando: Git push origin 'nome da branch criada'*

**Junção da Branch criada a qual foi desenvolvida a Feature**

*1º Comando: Git checkout master*

-> Volta para a Branch Padrão

*2º Comando: Git merge 'nome da branch a ser adicionada a padrão'*

->Merge -'Serve para mesclar commits e Branchs na Branch atual' por esse motivo é importante colocar o nome da branch logo após Git merge...
