# Como criar atalhos na área de trabalho (Desktop Entry)

```
sudo <editor de texto> /usr/share/applications <nome>.desktop
Exemplo:
sudo nano /usr/share/applications postman.desktop
```

* Agora, configure o atalho no editor:

```
Exemplo (remova TODOS os comentários abaixo e opcionais desnecessários na hora de configurar):
[Desktop Entry] # header indicando que é um atalho (obrigatório)
Version = 1.0 # Versão do app (optional)
Name = Postman # Nome do programa (obrigatório)
GenericName = Interface de teste de API # Nome comum do programa (optional)
Comment = IDE de teste # Descrição do programa (optional)
Exec =/home/nathan/Desktop/Postman/app/Postman  # Comando de inicialização do programa(obrigatório); 
Icon =/home/nathan/Desktop/Postman/app/logo.png  firefox # Icone do programa (obrigatório)
Terminal = false # Se roda no terminal ou não (optional); available when "Type" is set to "Application"
Type = Application # tipo do programa (obrigatório); possible values: "Application", "Link", etc.
Categories = Development;Application;Network; # Categorias para discernir nos menus de aplicações (optional)
```

<b>Importante:</b>o comando de inicialização deve ter permissão de execução pelo SO. Se não tiver, tente:
```
sudo chmod +x <executavel>
```
O arquivo final então deve ser no seguinte formato:

```
[Desktop Entry]
Name = Postman
GenericName = Interface de teste de API
Comment = IDE de teste
Exec =/home/nathan/Desktop/Postman/app/Postman
Icon =/home/nathan/Desktop/Postman/app/logo.png
Terminal = false
Type = Application
Categories = Development;Application;Network;
```

