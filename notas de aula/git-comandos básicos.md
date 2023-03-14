# Comandos Básicos de Git

## git config
A primeira coisa que você deve fazer quando instalar o Git é definir o seu nome de usuário e endereço de e-mail. Isso é importante porque todos os commits no Git utilizam essas informações, e está imutavelmente anexado nos commits que você realiza:

```bash
git config --global user.name "Danton"
git config --global user.email danton@exemplo.com
```

Você também pode adicionar um nickname (apelido) com o seguinte comando:

```bash
git config --global user.nickname "danton03"
```
</br>

## git init
Inicializa novo repositório do Git. Se você quiser colocar um projeto sob controle de revisão, este é o primeiro comando que você precisa inserir no terminal. Para isso, você precisa ir para o diretório do projeto e digitar:

```bash
git init
```

</br>

## git status
Ferramenta utilizada para observar quais arquivos estão em quais estados através do comando:

```bash
git status
```

</br>

## git add
Quando um repositório é inicialmente clonado, todos os seus arquivos estarão monitorados e inalterados porque você simplesmente os obteve e ainda não os editou. Conforme você edita esses arquivos, o Git passa a vê-los como modificados, porque você os alterou desde seu último commit. Você seleciona esses arquivos modificados e então faz o commit de todas as alterações selecionadas e o ciclo se repete.

### Monitorando Novos Arquivos
Para passar a monitorar um novo arquivo, use o comando git add. Por exemplo, para monitorar o arquivo README, você pode rodar isso:

```bash
git add README
```

Para adicionar mais de um arquivo ao monitoramento de uma vez só, você pode usar os seguintes comandos:

```bash
git add *
```

ou

```bash
git add .
```

</br>

## git commit
Armazena o conteúdo atual do índice em um novo commit, juntamente com uma mensagem de registro do usuário que descreve as mudanças.
Se usa o commit depois de já ter feito o git add, para fazer o commit:

```bash
git commit -m "Mensagem"
```

Para *commitar* também os arquivos versionados mesmo não estando no Stage basta adicionar o parâmetro -a :

```bash
git commit -a -m "Mensagem"
```

</br>

## git clone

Você clona um repositório da seguinte forma:

```bash
git clone url_do_projeto
```