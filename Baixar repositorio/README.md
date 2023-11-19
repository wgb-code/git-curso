# Baixar repositório (GIT CLONE)

Talvez o comando mais conhecido do git seja o de clonar um repositório, pois é com ele que podemos baixar quase todos os repositórios disponíveis no GITHUB e este processo é extremamente simples, necessitando de apenas uma linha de código o famoso:

```bash
    git clone +url_do_repositorio
```
Para você conseguir clonar um repositório basta usar o comando acima, vale ressaltar que você consegue encontrar o link HTTPS do repositório acessando o mesmo no GIT HUB, copiando toda sua URL do navegador (até mesmo o HTTPS://) e adicionando ao final dele o trecho .git, exemplo:

```bash
    git clone https://github.com/wgb-code/crud-php.git
```
Existem outras formas de clonar um repositório, como este curso é mostrando apenas o básico do básico irei mostrar de forma detalhada apenas a clonagem com a linkagem HTTPS, mas é importante ressaltar que existe os seguintes clones:

|  HTTPS |  SSH | GitHub CLI  |
|---------|---------|--------|
|Clonar através da URL| Clonar repositórios fechados, utilizando uma chave SSH gerada dentro do GITHUB  | Clonar para utilizar com o software GitHub CLI |

Como mencionado acima, este comando só irá funcionar em repositórios PÚBLICOS, por questão de segurança o GitHub bloqueia a clonagem de repositórios privados, caso você se torne um desenvolvedor em uma empresa, quando você for ter acesso ao repositório que irá trabalhar, muito provavelmente irá necessitar de uma ChaveSSH para completar a clonagem do repositório, esta chave é cadastrada dentro do GIT HUB EM:

```bash
    -> "Settings";
    -> No menu lateral esquerdo, "SSH and GPG Keys";
    -> Selecione a opção "New SSH key"
    -> Insira um nome a sua chave SSH para algo que faça sentido para o seu projeto
        ex: git-curso;
    -> Mantenha a opção "Authentication Key";
    -> Abaixo na opção "Key" você pode estar definindo manualmente uma chave ou deixar que o GitHub se encarregue de gera-la para você
```

### OBSERVAÇÃO!!!

Ao clicar em Add SSH Key, salve esta senha em algum local, pois ao atualizar ou sair desta tela, ela simplesmente irá sumir e você não irá conseguir verificar novamente no GitHub a senha ou nome da chave.