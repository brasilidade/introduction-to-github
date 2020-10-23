## Passo 4: Criar um branch

Vamos completar o primeiro GitHub flow (Fluxo do GitHub): criar um branch <sup>[:book:](https://help.github.com/articles/github-glossary/#branch)</sup>.

<details><summary>Criando um branch</summary>

## Creating a branch

:tv: [Video: Branches](https://www.youtube.com/watch?v=xgQmu81G1yY)

Você acabou de aprender como criar um branch—o primeiro passo no GitHub flow.

Branches são uma parte importante do GitHub flow porque eles nos permitem separar nossa trabalho da branch `main`.  Em outra palavras, o trabalho de todos está a salvo enquanto você contribui.


### Dicas ao usar branches

Um único projeto pode ter centenas de branches, cada uma sugerindo uma nova mudança para o branch `main`.

O melhor jeito de manter branches organizados com uma equipe é mantê-las concisos e breves. Em outras palavras, um único branch deve representar uma única funcionalidade ou um conserto de bug. Isso diminui a confusão entre contribuidores quando a branch é apenas ativo por alguns poucos dias antes dele ser mergeado <sup>[:book:](https://help.github.com/articles/github-glossary/#merge)</sup> com a branch `main`.

<hr>
</details>

### :keyboard: Atividade: Seu primeiro branch

{% if preferences.gitTool == 'cli' %}
1. Abra a interface de linha de comando de sua preferência, a qual nós chamaremos de shell a partir de agora.
1. Clone este repositório:
      ```shell
      git clone {{ thePayload.repository.clone_url }}
      ```
1. Navegue para o repositório no seu shell:
      ```shell
      cd {{ thePayload.repository.name }}
      ```
1. Crie um branch, dê o nome que achar melhor. Sinta-se à vontade para usar o nome sugerido abaixo.
      ```shell
      git branch my-slide
      ```
1. Dê push no branch para o GitHub:
      ```
      git push --set-upstream origin <NOME-DO-BRANCH>
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. Faça o download e abra o [Visual Studio Code](https://code.visualstudio.com/Download) (chamado de VS Code) caso ainda não o tenha feito.
1. No VS Code, abra a paleta de comandos usando <kbd>Ctrl+Shift+P</kbd> no Windows, ou <kbd>Command ⌘+Shift+P</kbd> no macOS. Você também pode seguir [Documentação oficial do VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository) na sessão `Cloning a repository`.
1. Digite: `git clone` e pressione <kbd>Enter</kbd>
      ![uma captura de tela do VS Code com a paleta de comandos aberta](https://user-images.githubusercontent.com/16547949/53639288-bcf9ec80-3bf6-11e9-9d18-d97167168248.png)
1. Cole a URL do repositório numa nova janela e pressione <kbd>Enter</kbd>:
      ```shell
      {{ thePayload.repository.clone_url }}
      ```
1. Selecione e diretório no qual você deseja salvar o repositório e clique em **Choose folder**. Então, abra o diretório selecionado.
1. O diretório do repositório agora deve estar aberto no seu projeto do VS Code.

 Clique em `main` no canto esquerdo da janela do VS Code. Isso vai abrir a Paleta de Comandos referente as branches do Git.
      ![uma captura de tela dos branches do Git no VS Code](https://user-images.githubusercontent.com/16547949/53639606-adc76e80-3bf7-11e9-98ac-bd41ae2b40db.png)
1. Clique em **Create new branch** e coloque o nome de branch que você quiser, por exemplo `my-slide`. Então pressione <kbd>Enter</kbd>.
1. Quando for perguntado para selecionar a ref de origem da branch, selecione `main`.
1. Clique na opção de controle de versão, clique na elipse (...) e selecione Push. Confirme a caixa de diálogo pedindo para você publicar o branch.
      ![uma captura de tela mostrando o controle de versão no VS Code](https://user-images.githubusercontent.com/16547949/53640015-ee73b780-3bf8-11e9-8c90-be9022b9555a.png)

{% else %}

1. Navegue para [Code tab]({{ thePayload.repository.html_url }})
2. Clique em **Branch: main** no drop-down
3. No campo, digite um nome para seu branch, por exemplo, `my-slide`
4. Clique em **Create branch: <name>** ou pressione a tecla <kbd>Enter</kbd> para criar seu branch

{% endif %}
<hr>
<h3 align="center">Eu vou responder quando detectar que um branch novo foi criada nesse repositório.</h3>
