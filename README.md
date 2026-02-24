# Como instalar/configurar o `JabRef` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para instalar/configurar o `JabRef` no `Linux Ubuntu`.

## _Abstract_

_This document contains the main commands and configurations to install/configure `JabRef` on `Linux Ubuntu`._

### Construído com

Esta seção deve listar todas as principais estruturas/bibliotecas usadas para inicializar seu projeto, bem como a sequência de instalação. Deixe quaisquer complementos/plugins para a seção de agradecimentos. Aqui estão alguns exemplos.

* [![Texlive](https://img.shields.io/badge/Texlive-3776AB?style=flat-square&logo=latex&logoColor=white)](https://tug.org/texlive/)

* [![JabRef](https://img.shields.io/badge/JabRef-44A833?style=flat-square&logo=latex&logoColor=white)](https://www.jabref.org/)

* [![Texstudio](https://img.shields.io/badge/Texstudio-008080?style=flat-square&logo=latex&logoColor=white)](https://www.texstudio.org/)

* [![MathPix](https://img.shields.io/badge/MathPix-008080?style=flat-square&logo=MathPix&logoColor=white)](https://mathpix.com/)

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>


## Descrição [2]

`JabRef`

O `JabRef` é um gerenciador de referências bibliográficas de código aberto desenvolvido para auxiliar pesquisadores, estudantes e autores na organização e gestão de suas bibliografias. Especialmente útil para trabalhos acadêmicos e científicos, o `JabRef` permite importar, organizar e formatar referências de maneira eficiente. Ele suporta uma variedade de formatos de arquivos bibliográficos, como BibTeX e EndNote, e oferece recursos como pesquisa avançada, autocompletar de campos, integração com bancos de dados online, bem como a capacidade de vincular arquivos PDF às entradas de referência. Com sua interface amigável e recursos poderosos, o `JabRef` é uma escolha popular para quem precisa manter sua bibliografia organizada e criar citações precisas em seus documentos acadêmicos.


## 1. Configurar/Instalar/Usar o `JabRef` no `Linux Ubuntu` [1]

Para configurar/instalar/usar o `JabRef` no `Linux Ubuntu`, você pode seguir os seguintes passos:

1. Abrir o `Terminal Emulator`. Você pode fazer isso pressionando:

    ```bash
    Ctrl + Alt + T
    ```


2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando:
    ```bash
    sudo apt clean
    ```

    2.2 Remover pacotes `.deb` antigos ou duplicados do `cache` local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando:
    ```bash
    sudo apt autoclean
    ```

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando:
    ```bash
    sudo apt autoremove -y
    ```

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt update
    ```

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes:
    ```bash
    sudo apt --fix-broken install
    ```

    2.6 Limpar o `cache` do gerenciador de pacotes `apt` novamente:
    ```bash
    sudo apt clean
    ```

    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt list --upgradable
    ```

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt full-upgrade -y
    ```

3. **Instale o `JabRef`**: Você pode instalar o TeX Studio diretamente a partir dos repositórios oficiais do Ubuntu usando o comando apt. Execute o seguinte comando para instalar:

    ```bash
    sudo snap install jabref
    ```

## Código completo para configurar/instalar/usar o `JabRef` no `Linux Ubuntu`

Para configurar/instalar/usar o `JabRef` no `Linux Ubuntu` sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abrir o `Terminal Emulator`. Você pode fazer isso pressionando:

    ```bash
    Ctrl + Alt + T
    ```

2. Digite o seguinte comando e pressione `Enter`:

    ```bash
    sudo apt clean
    sudo apt autoclean
    sudo apt autoremove -y
    sudo apt update
    sudo apt --fix-broken install
    sudo apt clean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo snap install jabref
    jabref --version
    ```

## Referências

[1] OPENAI. ***Instalar o `jabref` no `linux ubuntu` pelo `terminal emulator`.*** Disponível em: <https://chatgpt.com/c/ca891d3e-e50e-4adb-9baf-708bfa6d1632> (texto adaptado). ChatGPT. Acessado em: 14/11/2023 18:56.

[2] JABREF. ***Installation.*** Disponível em: <https://docs.jabref.org/installation#installation-instructions> (texto adaptado). ChatGPT. Acessado em: 29/09/2023 20:09.

[3] OPENAI. ***VS code: editor popular.*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado). ChatGPT. Acessado em: 14/11/2023 18:56.

