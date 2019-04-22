# Dicas sobre git

**Índice**   
1. [Criando repositorio centralizado - ha-rpi3](#id1)
2. [Samba share](#id2)
3. [Mosquitto broker](#id3)

## Criando repositorio centralizado - ha-rpi3<a name="id1"></a>
ha-rpi3

### Criando o repositorio vazio
````
cd D:\development\repo\ha-rpi3
git init --bare
````

## Exemplo desenvolvedor 1

### Clonado o repositorio raiz e abrindo diretorio
```
git clone cd D:\development\repo\ha-rpi3
cd ha-rpi3
```

### Colocando arquivos no reposito local e depois colocando as alterações para o repositorio raiz
```
# adiciona os arquivos no reposito
git add .

# validando os arquivos
git commit -m "primeira versionamento"

# verificando o status
git status

# verifica os repositorios remotos
git remote -v

# coloca uma nova versao dos arquivos no repositorio remoto ha-rip3
git push origin master
```


## Exemplo desenvolvedor 2

### fazendo macete para levar o arquivos .git para o diretorio z:\
```
# fazendo uma copia do repositorio raiz
git clone d:\development\repo\ha-rpi3

# copiando o arquivo .git para o z:\
# depois de copiar ir para z:\ e executar:
git reset -–hard

```

## Exemplo desenvolvedor 2

### fazendo macete para levar o arquivos .git para o diretorio z:\

```
# pega nova versao do repositorios
git pull origin master

```




