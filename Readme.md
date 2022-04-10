*Olá meu nome é Kelvin e esse simples Arquivo/Projeto tem como objetivo de deixar relatado os conceitos do Git.*

*O QUE É : Git é um sitemas de controle de versões*
-> Git registra as mudanças que ocorrem no código-fonte de um projeto.

-> Logo, permite que os arquivos sejam alterados de forma simultânea, por inúmeras pessoas, sem a preocupação que essas alterações sejam sobrescritas umas pelas outras.

 *Vantagens:*
-> A sua 'arquitetura descentralizada' é o que faz com que o Git seja diferenciado em relação às outras opções de sistemas similares, não existe um repositório oficial, embora isso possa ser feito. Sendo assim, em cada repositório, incluindo o da máquina do contribuidor, vai existir uma cópia completa e funcional, permitindo a utilização das operações mesmo offline.

 *Desvantagem:*
-> Uma das grandes desvantagens desse tipo de arquitetura é a baixa performance gerada caso tenha muitas equipes e projetos em um mesmo repositório. Além disso, é preciso estar sempre on-line para realizar as operações, como criar as ramificações. 

 *Qual a importância do Git ?*
-> A importancia do Git é grande, quando se tem +1 pessoa para se trabalhar no desenvolvimento de um codigo se utiliza o Git fazendo uma nova versão do codigo acada acrecimo de linhas deixando atualizado com um novo versionamento e caso ocorra algo inesperado é facil de voltar a versão do codigo para uma antecessora. 

*Como que o Git funciona ?*
Git trabalha em uma arquitetura em Branch (ou ramificações). 
Cada novo commit, ou seja, alteração do código, cria um novo ponto na ramificação atual (uma branch).

*1º Comando: Git init* 
->  cria um repositorio vazio(Uma pasta que iremos armazenar o nosso codigo) & cria uma breanch (Master) 'linha do tempo de versões principais em uma linha coronologica'.

Tecnica e conhecimento: Uma boa pratica é criar uma nova ramificação, se por exemplo estivermos um Software grande e acada alteraçao que formos fazer for ficar na "Master" seria diversas versões, então para uma melhor pratica criar ramificação e atualizar a master logo ter terminado a alteração e proporcionando um bom controle de versão é uma otima pratica.

*2º Comando: Git add arquivo ou . caso seja todos*
->adiciona na area de staging(staging area permite que seja realizado vários commits a partir dela.) uma area que o arquivo ira ficar aguardando o commit e O comando git add mantém o histórico de todas as ações realizadas no código, permitindo que, se algum problema ocorrer na aplicação, o comando de desfazer alteração possa ser acionado. 

*3º Comando: Git status*
-> mostra se tem atualizaçoes feita no arquivo que devem ser comitadas afim de criar uma versão.

*4º Comando: Git -m commit "mensagem para informação do que foi alterado"*
-> salva a nova versao do seu arquivo 

