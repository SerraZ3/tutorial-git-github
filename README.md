[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

# Tutorial Git e Github

Tutorial de como usar Git e Github

Não esqueça de deixar seu star :star: no repo :grin:

## O que é git e github

Git é uma ferramenta para versionamento de código e o Github é uma plataforma para armazenar o versionamento do código.

Cuidado para não confundir, Git e Github não são a mesma coisa! Enquanto o git é toda a ferramenta de versionamento, o github é uma plataforma que serve para compartilhar e salvar o código na núvem. Além do github existem outra como [GitLab](https://gitlab.com/users/sign_in), [GitBucket](https://bitbucket.org/), entre outras.

## Antes de começar

Um projeto que está configurado com o Git possui sempre o arquivo `.git`. Para verificar se ele existe você pode rodar o seguinte comando no terminal

```shellscript
$ ls -a
```

ou

```shellscript
$ ls -la
```

Um projeto que está vinculado a um repositório no Github, Gitlab, ou qualquer outra plataforma remota possui sempre um origin. Para verificar basta rodar o seguinte comando na pasta desejada

```shellscript
$ git remote get-url origin
```

## Comandos

### Init

Adiciona o arquivo `.git`. Esse comando só deve ser dado caso o arquivo não exista. Para verificar olhe [antes de começar](#antes-de-começar)

```shellscript
$ git init
```

### Status

Comando que mostra a situação (ou status) dos arquivos no branch atual. Se tiver arquivos modificados, deletados, novos ou com conflitos ele irá mostrar quais são.

```shellscript
$ git status
```

### Add

Esse comando adiciona um ou mais arquivos para ser registrado no comando `commit`.

Adiciona todos os arquivos que foram alterados:

```shellscript
$ git add .
```

Adiciona apenas um arquivo

```shellscript
$ git add NOME_ARQUIVO
```

### Commit

Registra todos os arquivos que foram previamente adicionados com o comando [Add](#add)

```shellscript
$ git commit -m "Mensagem das alterações realizadas"
```

### Push

Comando que serve para enviar registros realizado pelo [Commit](#commit).

```shellscript
$ git push origin NOME_DA_BRANCH
```

**Atenção:** É necessário estar com o repositório remoto vinculado, para verificar olhe [antes de começar](#antes-de-começar)

### Pull

Comando que verifica se o repositório remoto possui algum [Commit](#commit) a frente do seu. Se houver ele vai pegar ele e trazer para seu máquina.

```shellscript
$ git pull origin NOME_DA_BRANCH
```

### Branch

Gerencia as branchs do seu repositório.

Abaixo, lista todas as branchs em sua máquina e diz qual você está atualmente. Para sair da tela que ele mostra basta clica no `q` do seu teclado

```shellscript
$ git branch
```

Cria uma nova branch

```shellscript
$ git branch NOME_NOVA_BRANCH
```

### Checkout

Serve para navegar entre os branchs

Abaixo, muda de branch

```shellscript
$ git checkout NOME_DA_BRANCH
```

Cria uma branch caso não exista e muda para essa branch

```shellscript
$ git checkout -b NOME_DA_BRANCH
```

### Merge

Pega o conteúdo de outro branch e mescla com o seu branch atual

```shellscript
$ git merge NOME_DO_OUTRO_BRANCH
```

[contributors-shield]: https://img.shields.io/github/contributors/SerraZ3/tutorial-git-github.svg?style=for-the-badge
[contributors-url]: https://github.com/SerraZ3/tutorial-git-github/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/SerraZ3/tutorial-git-github.svg?style=for-the-badge
[forks-url]: https://github.com/SerraZ3/tutorial-git-github/network/members
[stars-shield]: https://img.shields.io/github/stars/SerraZ3/tutorial-git-github.svg?style=for-the-badge
[stars-url]: https://github.com/SerraZ3/tutorial-git-github/stargazers
[issues-shield]: https://img.shields.io/github/issues/SerraZ3/tutorial-git-github.svg?style=for-the-badge
[issues-url]: https://github.com/SerraZ3/tutorial-git-github/issues
[license-shield]: https://img.shields.io/github/license/SerraZ3/tutorial-git-github.svg?style=for-the-badge
[license-url]: https://github.com/SerraZ3/tutorial-git-github/blob/master/LICENSE
