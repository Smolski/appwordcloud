# APPWORDCLOUD

Este é um aplicativo criado via RStudio que permite que o usuário carregue sua própria base de dados (em formato UTF-8) e crie sua própria núvem de palavras e tenha a liberdade de escolher dentre algumas opções de text minig como será a nuvem desejada.

### Instruções

**Input da base de dados**

Para dar início a construção da nuvem de palavras selecione o arquivo (em formato csv com codificação UTF-8) que contenha apenas duas colunas em que:

    * Coluna1: usuario
    * Coluna2: texto

[exemplo de base](https://github.com/gomesfellipe/appwordcloud/blob/master/base.csv)

**Stopwords**

Para remover palavras da nuvem de palavras (chamadas de stopwords), basta inseri-las, separadas por vírgula, na caixa "**Removendo palavras**". Exemplo de como devem ser incluidas as palavras:

     nao, dele, dela, nos

**Sentimentos**

Na opção "**Marque se deseja usar cor para sentimentos**" a cor da nuvem é baseada em um dicionário léxico do qual um conjunto de palavras já foram pré-classificadas como positiva, negativa ou neutra.


[Codigo no github](https://github.com/gomesfellipe/appwordcloud/blob/master/appwordcloud.Rmd)

**Importante**: Para utilizar a transformação tf-idf em conjunto com a remoção de sufixos, o procedimento deve ser feito na ordem: 

    Text Stemming > tf-idf
