# Como verificar se o SO reconhece seu disco removível (i.e. pen drive, hd externo):
Com o disco desconectado:
```
$ cd /dev/
$ ls | grep sd
```
Agora, com o disco conectado:
```
$ cd /dev/
$ ls | grep sd
```
Só checar as diferenças (se houverem) entre as saídas. Se não houver diferença, o sistema não está reconhecendo o disco.

