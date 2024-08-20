# Instalando o Flutter

## 1. Verificar os Requisitos do Sistema

**Hardware:**

| Requisito | Minimo | Recomendado |
| :--------- | :------: | :-----------: |
| x86_64 núcleos de CPU | 4 | 8 |
| Memória RAM | 8GB | 16GB |
| Espaço em Disco | 11GB | 60GB |
| Resolução da tela em pixels	| WXGA (1366 x 768)	| FHD (1920 x 1080) |

**Outros Requisitos Necessários**: 

- Windows 10 ou superior (64 bits).
- Windows PowerShell 5 ou superior.
- Git para Windows 2.27 ou superior.
- Android Studio 2023.3.1 (Jellyfish) ou superior (O flutter requer a versão completa do Android Studio).

## 2. Instalar o SDK do Flutter

1. Baixe o pacote de instalação a seguir para obter a versão estável mais recente do Flutter SDK.
2. Crie um diretório onde você possa instalar o Flutter (considere criar uma paste em: `C:\Users\{username}` ou `C:\Users\{username}\AppData\Local`).
3. Extraia o arquivo para o diretório que você acabou de criar (quando terminar, o SDK do Flutter deve estar em um diretorio como: `C:\user\{username}\dev\flutter`).

## 3. Atualizar Variáveis de Ambiente do Windows

1. Abra o Painel de Controle e vá até **Sistema e Segurança** > **Sistema** > **Configurações Avançadas do Sistema**.
2. Na aba Avançado, clique em **Variáveis de Ambiente**.
3. Na seção **Variáveis de usuário para (*nome de usuário*)**, Selecione a entrada **Path** e clique em **Editar**.
4. Clique em **Novo** e adicione o caminho para o diretório `\flutter\bin` (por exemplo, `C:\user\{username}\dev\flutter\bin`).
5. Selecione a entrada que acabou de adicionar e clique em **Mover para cima** até que ela esteja no topo da lista.
6. Clique em **Ok**.
7. Para habilitar essas alterações, feche e reabra todos os prompts de comando e instâncias do PowerShell existentes.

## 4. Configurar o Android Studio

1. Inicie o Android Studio.
2. Siga o assistente de configuração do Android Studio.
3. Instale os seguintes componentes:
    - Plataforma Android SDK, API 35.0.1
    - Ferramentas de linha de comando do SDK do Android
    - Ferramentas de compilação do SDK do Android
    - Ferramentas da plataforma Android SDK
    - Emulador Android
4. Configure um dispositivo virtual (emulador).

## 5. Concordar com as Licenças do Android

1. Execute o seguinte comando para habilitar a assinatura de licenças:  
  ```
    flutter doctor --android-licenses
  ```

2. Se tudo ocorrer bem, a seguinte mensagem deve ser retornada:  
  ```
    All SDK package licenses accepted.
  ```

## 6. Executar Flutter Doctor

Para verificar se os componentes foram instalados corretamente, execute o seguinte comando:
```
  flutter doctor
```

A seguinte mensagem será retornada:
```
  Running flutter doctor...
  Doctor summary (to see all details, run flutter doctor -v):
  [✓] Flutter (Channel stable, 3.24.0, on Microsoft Windows 11 [Version 10.0.22621.3155], locale en)
  [✓] Windows version (Installed version of Windows is version 10 or higher)
  [✓] Android toolchain - develop for Android devices (Android SDK version 35.0.1)
  [!] Chrome - develop for the web
  [!] Visual Studio - develop Windows apps
  [✓] Android Studio (version 2024.1)
  [✓] VS Code (version 1.92)
  [✓] Connected device (1 available)
  [✓] Network resources

  ! Doctor found issues in 2 categories.
```

!!! info "Observação" 
    Alguns componentes podem ser opcionais, como **Visual Studio Code** e o **Chrome**.