
# CURSO DE GIT


Neste repositório, abordarei os conhecimentos que adquiri ao longo do tempo por meio de diversos cursos de GIT & GITHUB. Abordarei desde o uso mais simples, como clonar um repositório e subir atualizações, até conceitos mais avançados e explicações teóricas. É importante ressaltar que não sou professor e estou utilizando este repositório para aprofundar o meu aprendizado.



## Instalação

O primeiro passo para utilizar o Git é instalá-lo na máquina. Neste repositório, não aprofundarei a instalação, pois é um processo simples e a própria documentação já oferece auxílio. No entanto, para fins de esclarecimento, informo que, ao instalar o Git, atenho-me às seguintes observações:


```bash
Na opção "Selecionar componentes", seleciono:
        
    -> Integração com o Windows Explorer;
        -> Git Bash aqui;
        -> Git GUI aqui.

Geralmente, essas opções já vêm pré-selecionadas, mas é sempre importante verificar se estão, de fato, selecionadas.

Na opção "Escolha o editor padrão usado pelo Git", seleciono a seguinte opção:

    "Usar o Visual Studio Code como editor padrão do Git".

Como utilizo o VSCODE como IDE, é importante ressaltar que é necessário marcar a versão "default editor" e não a "insiders".
```
De resto, mantenho tudo padrão e, se necessário, configuro posteriormente usando o próprio Git Bash. Para saber mais sobre a instalação do Git, basta acessar o site:

https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

    
## Configurando o Git e Váriaveis de ambiente

Após termos o Git instalado, devemos configura-lo. em meu caso irei criar uma pasta no meu Windows especifica para este curso nomeada de: "git-curso", após isto, irei clicar com o botão direito em cima dela e selecionar a opção "Open git bash here".

As primeiras alterações que devemos realizar em nosso git é a configuração de nosso nome de usuário e email.

Para isto, devemos nos atentar se iremos querer salvar estas informações de forma:

|  GLOBAL |  SYSTEM | LOCAL  |
|---------|---------|--------|
|para utilizar em todos os repositórios   | para utilizar em todos os usuários existentes na máquina  | Para utilizar apenas em um repositório especifico  |

Para definirmos nosso nome e email no git iremos usar a variavel global, pois neste caso eu quero utilizar as mesmas informações para todos os repositórios.

Para isto irei utilizar o seguinte comando:

```
    git config --global user.nome "seu nome";
    git config --global user.email seu email;
```
Para certificarmos que nosso nome e e-mail estão configurados, basta digitarmos novamente os comandos até user.nome/user.email que o git irá nos retornar as informações salvas.
## Mais configurações e Branch

Branch é um assunto que irá acompanhar sua vida de desenvolvedor para sempre, mas o que é branch? em resumo, brench é uma ramificação do código, ou seja, o próprio GIT nos disponibiliza uma branch chamada "main" esta é nossa linha principal, é nela que iremos subir nosso código após trabalharmos nele, testarmos e por ai vai... É o nosso código final (claro que poderá haver bugs mesmo após o mesmo já estar em operação).

Mas em um contexto normal trabalhamos em cima de diversas branchs, exemplo: desenvolvedor (o nome pode variar de acordo com o seu local de trabalho), nesta branch "desenvolvedor" iremos realizar todas as implementações de nosso código, sem afetar o que ja foi feito (e está na branch main), após, iremos testar nosso código desenvolvido em outra branch exclusiva para testes e posteriormente após estar tudo pronto o código é movido para a nossa branch principal no caso, a main.

### Como configurar e criar novas Branch's

Primeiramente temos que configurar nossa branch principal para "main", este processo pode ser realizado também na instalação do git mas irei fazer via Git Bash:

```
    git config --global init.defaultBranch main
```
Para criarmos uma branch o processo é bem simples:

```
    git init     //para iniciar um repositório git
    git checkout -b nome_da_branch    //Verificar aonde você quer salvar essa branch (global, system, local)
```
Verificar todas as branchs do seu repositório:

```
    git branch
```

Mais instruções referente ao uso do GIT irá se encontrar dentro das pastas deste repositório, as pastas estarão organizadas conforme o conteúdo passado.
