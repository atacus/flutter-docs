# Criando seu Primeiro App em Flutter

!!! info "Observação" 
    Este exemplo utiliza o **Visual Studio Code** como IDE,  mas se quiser também pode utilizar o Android Studio (basta ter memória RAM suficiente).

## 1. Acessar Extensões do Visual Studio Code
- Com o Visual Studio Code aberto, no menu lateral, selecione a aba “extensões”:

## 2. Instalar Plugin
- No campo de busca, digite “Flutter”. O primeiro resultado da busca será o plugin oficial. Clique no pequeno botão “Install” verde. O plugin já contém tudo que precisamos para executar e debugar nosso código Dart.

![visualstudio.png](https://arquivo.devmedia.com.br/naoexclusivo/CaioRolla/sala-flutter/artigos/009.png){ align=center }
!!! info "Tudo Pronto" 
Finalmente podemos criar nosso primeiro aplicativo em Flutter!

## 3. Criando um aplicativo com Flutter

1. Com o SDK instalado e adicionado à variável de ambiente “Path”, criar um novo projeto Flutter é extremamente simples. Para isso, no terminal do Windows, navegue até o diretório onde deseja iniciar o seu projeto e execute o seguinte comando:   
  ```
    flutter create meu_primeiro_app
  ```
!!! info inline end "Nome do Projeto"

    O parâmetro meu_primeiro_app é o nome da nossa aplicação. Sinta-se livre para colocar o nome que quiser.


2. O Flutter ficará encarregado de criar todos os arquivos aplicação. Feito isso, ainda no terminal, navegue até o diretório que foi criado pelo CLI: 
```
  cd meu_primeiro_app
```

3. Para abrir o projeto no Visual Studio Code basta executar o comando:
```
  code .
```

