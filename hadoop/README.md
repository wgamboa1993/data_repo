# Guia rapida instalación Hadoop


## Instalación de todos los servicios necesarios

Esta es un archivo bootstrap, el cual trae la instalación y configuración de:

- java8
- hadoop.3.1.2
- python3.7
- pip3
- git
- awscli


## Workdir directorio raiz del usuario.

```
sudo apt-get install wget
wget https://raw.githubusercontent.com/Christianivh/data_repo/master/hadoop/bootstrap1.sh -O boostrap.sh
bash boostrap.sh "$(whoami)"

```

## Inicio Hadoop

Una vez finalizada la instalación de hadoop, proceda a formatear

```{shell}
source ~/.bashrc

cd hadoop

hdfs namenode –format
```


## Iniciar Servicios

Proceda a iniciar los servicios de HDFS / YARN /

```{shell}
sbin/start-all.sh

sbin/mr-jobhistory-daemon.sh start historyserver
```

copyright!
