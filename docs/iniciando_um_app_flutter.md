# Iniciando um App Flutter

=== "Visual Studio Code"

    !!! info "Observação" 
        Este exemplo utiliza o **Visual Studio Code** como IDE,  mas se quiser também pode utilizar o Android Studio (basta ter memória RAM suficiente).

    ## Configurando o Visual Studio Code

    1. Com o Visual Studio Code aberto, no menu lateral, selecione a aba "extensões".

    2. No campo de busca, digite "Flutter". O primeiro resultado da busca será o plugin oficial. Clique no pequeno botão "Install" na cor verde. O plugin já contém tudo que precisamos para executar e debugar nosso código Dart.

    ![visualstudio.png](https://arquivo.devmedia.com.br/naoexclusivo/CaioRolla/sala-flutter/artigos/009.png)

    !!! success "Tudo Pronto" 
        Finalmente podemos criar nosso primeiro aplicativo em Flutter!

    ## Iniciando um Novo App

    1. No terminal do Windows, navegue até o diretório onde deseja iniciar o seu projeto e execute o seguinte comando:   
    ``` { .powershell .copy }
      flutter create meu_primeiro_app
    ```
    
    2. O Flutter ficará encarregado de criar todos os arquivos da aplicação. Feito isso, ainda no terminal, navegue até o diretório que foi criado pelo CLI: 
    ``` { .powershell .copy }
      cd meu_primeiro_app
    ```

    3. Para abrir o projeto no Visual Studio Code basta executar o comando:
    ``` { .powershell .copy }
      code .
    ```

=== "Terminal"

    1. Para iniciar um novo aplicativo em Flutter, execute o seguinte comando:
    ``` { .powershell .copy }
      flutter create meu_primeiro_app
    ```

    2. Navegue para o diretório criado:
    ``` { .powershell .copy }
      cd meu_primeiro_app
    ```

    3. Verifique se você possuí um dispositivo de destino (emulador) em execução:
    ``` { .powershell .copy }
      flutter devices
    ```
        - Caso não tenha, abra o Android Studio, configure e inicie um novo emulador.

    4. Por fim, para iniciar seu aplicativo, execute o seguinte comando:
    ``` { .powershell .copy }
      flutter run
    ```

## Resultados

Se tudo ocorreu bem, você terá um aplicativo inicial semelhante a esse:

<figure markdown="span">
  ![Aplicativo inicial Flutter](./assets/app_demo.png){ width=500 }
</figure>

E uma estrutura de diretórios assim:

<figure markdown="span">
  ![Estrutura de pastas de um app Flutter](./assets/lista_de_diretorios.png)
</figure>

!!! tip "Dica"
    A maior parte dos arquivos do seu aplicativo se encontram no diretório `lib` e provavelmente é la que você passará a maior parte do tempo.


## Código Base

Agora, para iniciar o desenvolvimento de um app, precisamos criar um arquivo `main.dart` no diretório `lib` e adicionar uma função `main`, como no exemplo a seguir:

``` { .dart .copy }
import "package:flutter/material.dart";

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: "Meu Primeiro App", 
      home: InitialPage(),
    );
  }
}

void main(){
  runApp(const MyApp());
}
```

Aqui temos, além da função `main`, a classe `MyApp`, que é nosso **widget** inicial, onde a partir dele, temos nosso ponto de entrada para o resto da aplicação. No exemplo acima, o atributo `home` recebe um objeto `InitialPage()`, que é um widget com a implementação da página inicial, que por sua vez terá a chamada de diversos outros widgets. Veja mais sobre widgets [aqui](/widgets).