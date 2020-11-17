# Force

## Executando 
docker-compose run force bash

## Adquirindo Metadados 
force-level1-csd -u /metadata

## Verificando imagens disponíveis

A função para executar o download das imagens é:

```
force-level1-csd
```

Informe que será executado somento uma verificação sobre as imagens disponíveis: 

```
-n
```

Informe o diretório que ficaram os metadados: 

```
./metadata
```

Informe o arquivo que terá o metadados, nesse caso foi utilizado o landsat: 

```
./metadata/metadata_landsat.csv
```

Informe o arquivo que armazenará o log dos arquivos baixados: 

```
./lista/l-1-datapool.txt
```

Informe a área, nesse caso foi utilizado o Path Row, as imagens serão armazenadas em um diretório com esse nome:

```
226068
```

Informe a porcentagem de núvens:

```
0,10
```

Informe o intervalo do período desejado:

```
20140101,20201110
```

Comando completo:
```
force-level1-csd -n /metadata /metadata/metadata_landsat.csv, /lista/l-1-datapool.txt 226068 -c 0,10 -d 20140101,20201110
```