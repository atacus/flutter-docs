# Iniciando um App Flutter

1. Para iniciar um novo aplicativo em Flutter, execute o seguinte comando:
``` { .powershell .copy }
  flutter create app_teste
```

2. Navegue para o diretório criado:
``` { .powershell .copy }
  cd app_teste
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

![Aplicativo inicial Flutter](./assets/app_demo.png){ width=500 }

E uma estrutura de diretórios assim:

![Estrutura de pastas de um app Flutter](./assets/lista_de_diretorios.png)

!!! tip "Dica"
    A maior parte dos arquivos do seu aplicativo se encontram no diretório `lib` e provavelmente é la que você passará a maior parte do tempo.
