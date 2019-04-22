# Hass.io - Instalaçãp de add-on

**Índice**   
1. [Instalando SSH server](#id1)
2. [Samba share](#id2)
3. [Mosquitto broker](#id3)

## Instalando  SSH server<a name="id1"></a>
Logar no Home Assistant - opções Hassio.io/ADD-ON Store / SSH server

Config:
````
{
  "authorized_keys": [],
  "password": "password"
}
````
SSH serve / start


## Instalando  Samba share<a name="id2"></a>
Logar no Home Assistant - opções Hassio.io/ADD-ON Store / Samba share

Config:
````
{
  "workgroup": "SeuGrupo",
  "username": "usuario",
  "password": "senha",
  "interface": "",
  "allow_hosts": [
    "10.0.0.0/8",
    "172.16.0.0/12",
    "192.168.0.0/16"
  ]
}
````
Samba share / start


## Instalando  Mosquitto broker<a name="id3"></a>
Logar no Home Assistant - opções Hassio.io/ADD-ON Store / Mosquitto broker 

Config:
````
{
  "logins": [
    {
      "username": "<usuario>",
      "password": "<senha>"
    }
  ],
  "anonymous": false,
  "customize": {
    "active": true,
    "folder": "mosquitto"
  },
  "certfile": "fullchain.pem",
  "keyfile": "privkey.pem"

````

Como foi habilitado a opção customize / active "true"

Precisammos acessar  o compartilhamento do windows para criar o diretorio de configuracao do mosquitto via samba. 

ex.:
```
win + r (acessar o executar)
\\<ip>\share
criar o diretorio 
mosquitto
```

Mosquitto broker  / start

