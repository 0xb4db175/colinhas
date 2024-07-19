# host

Comando `host`.

## Pesquisa simples

Retorna os registros A, AAAA e MX associados a um domínio

`host example.com`

## Especificar um tipo de registro

`host -t A exampĺe.com`

## Especificar um servidor de DNS

`host example.com 8.8.8.8`

## Realizar uma busca reversa

`host 192.0.2.0`

## Principais Flags

* `-4`: Usar apenas IPv4 no transporte da consulta.
* `-6`: Usar apenas IPv6 no transporte da consulta.
* `-a`: Equivalente a `-v -t ANY`.
* `-C`: Comparar registros SOA em servidores de nome autoritativos.
* `-l`: Listar a zona, ou seja, realizar uma transferência da zona especificada e mostrar todos os registros NS, PTR, A e AAAA.
* `-la`: O mesmo que `-l`, porém mostrando todos os registros da zona.
* `-p`: Especificar a porta do servidor DNS.
* `-t`: Especificar o tipo de registro a ser consultado.
* `-T`: Modo TCP.
* `-U`: Modo UDP (usado por padrão).
* `-v`: Resposta detalhada (modo verboso).

Para mais opções, ver `host -h` (ou simplesmente `host`) e `man host`.
