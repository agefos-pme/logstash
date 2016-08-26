# Configuration Logstash

Ce projet décrit la configuration des inputs suivants:
- ssh
- yum
- netflow (cisco)
- kaspersky
- activedirectory
- squid
- switchs HP
- palo alto

On retrouvera dans les sous répertoires les informations suivantes:

| repetoire | contenu |
|---|---|
| conf.d | Configuration des filtres input/filter
| geoip | Geolocalisation pour palo alto / squid / cisco
| patterns | Log message pattern matching
| templates | Templates output pour communication logstash - elasticsearch

## Installation des fichiers de configuration

Pour ce faire, il faut disposer des fichiers de configuration de logstash et de la définition du conteneur qui se trouve dans le projet [rancher-catalog](/agefos-pme/rancher-catalog/templates/logstash/).

Pour ce faire, il suffit de:

![Etape1](/docs/etape1.png)

![Etape2](/docs/etape2.png)

## Installation en ligne de commande

Se connecter sur l'hôte:

```shell
# # Si cela n'a pas été fait auparavant
# git clone https://github.com/agefos-pme/rancher-catalog
# cd rancher-catalog/templates/logstash/0
# rancher-compose up -d
```
