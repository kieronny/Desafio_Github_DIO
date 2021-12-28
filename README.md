# Desafio_Github_DIO
Criando seu Primeiro Repositório no GitHub Para Compartilhar Seu Progresso

#Links Uteis
- [React](https://aboutreact.com/react-native-app-intro-slider/)

OBS: repositório criado para entrega do desafio.

#GUIA PRÁTICO

Apenas um guia prático para começar com git. sem complicação ;)

Instalação
- Baixe o git para OSX(http://git-scm.com/download/mac)
- Baixe o git para Windows(http://msysgit.github.io/)
- Baixe o git para Linux(http://book.git-scm.com/2_installing_git.html)

[Criando um novo repositório]
crie uma nova pasta, abra-a e execute o comando
#git init

[Obtenha um repositório}
crie uma cópia de trabalho em um repositório local executando o comando
#git clone /caminho/para/o/repositório
quando usar um servidor remoto, seu comando será
#git clone usuário@servidor:/caminho/para/o/repositório

[fluxo de trabalho]
seus repositórios locais consistem em três "árvores" mantidas pelo git. a primeira delas é sua Working Directory que contém os arquivos vigentes. a segunda Index que funciona como uma área temporária e finalmente a HEAD que aponta para o último commit (confirmação) que você fez.

[Aicionar & confirmar]
Você pode propor mudanças (adicioná-las ao Index) usando
#it add <arquivo>
#it add *
Este é o primeiro passo no fluxo de trabalho básico do git. Para realmente confirmar estas mudanças (isto é, fazer um commit), use
#git commit -m "comentários das alterações"
Agora o arquivo é enviado para o HEAD, mas ainda não para o repositório remoto.
  
[Enviando alterações]
Suas alterações agora estão no HEAD da sua cópia de trabalho local. Para enviar estas alterações ao seu repositório remoto, execute
git push origin master
Altere master para qualquer ramo (branch) desejado, enviando suas alterações para ele.

Se você não clonou um repositório existente e quer conectar seu repositório a um servidor remoto, você deve adicioná-lo com
git remote add origin <servidor>
Agora você é capaz de enviar suas alterações para o servidor remoto selecionado.
  
[Ramificando]
Branches ("ramos") são utilizados para desenvolver funcionalidades isoladas umas das outras. O branch master é o branch "padrão" quando você cria um repositório. Use outros branches para desenvolver e mescle-os (merge) ao branch master após a conclusão.
  
[Crie um novo branch chamado "funcionalidade_x" e selecione-o usando]
#git checkout -b funcionalidade_x
retorne para o master usando
#git checkout master
e remova o branch da seguinte forma
#git branch -d funcionalidade_x
um branch não está disponível a outros a menos que você envie o branch para seu repositório remoto
#git push origin <funcionalidade_x>
  
[Atualizar & mesclar]
para atualizar seu repositório local com a mais nova versão, execute
git pull na sua pasta de trabalho para obter e fazer merge (mesclar) alterações remotas.
para fazer merge de um outro branch ao seu branch ativo (ex. master), use
git merge <branch>
