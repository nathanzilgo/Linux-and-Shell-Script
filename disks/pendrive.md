# Como verificar se o Ubuntu reconhece seu pen drive:
### Com o disco desconectado:
$ cd /dev/
$ ls | grep sd
### Agora, com o disco conectado:
$ cd /dev/
$ ls | grep sd
## Só checar as diferenças (Se houverem) entre as saídas. Se não houver diferença, o sistema não está reconhecendo o disco.

