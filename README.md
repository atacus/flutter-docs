## flutter-docs

> Qual linguagem de programação o Flutter usa?
> O Flutter usa a linguagem de programação de código aberto Dart, que também foi desenvolvida pelo Google. A linguagem Dart é otimizada para o desenvolvimento de interfaces de usuário e muitos dos pontos fortes dela são usados no Flutter.

#Editar arquivo daemon

```
vim /etc/systemd/system/mkdocs.service

```

# Recarregar o Systemd para reconhecer o novo serviço

```
systemctl daemon-reload

```
# Iniciar o serviço

```
systemctl start mkdocs.service

```
# Habilitar o serviço para iniciar automaticamente na inicialização do sistema

```
systemctl enable mkdocs.service

```
# Verificar o estado do serviço. 

```
systemctl status mkdocs.service

```

# Parar o serviço

```
systemctl stop mkdocs.service

```

# Desabilitar o serviço

```
systemctl disable mkdocs.service

```

# Log dos sitemas 

```
journalctl -u mkdocs.service
```

```
```
