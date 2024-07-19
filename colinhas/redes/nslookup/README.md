# nslookup

Comando `nslookup`.

## Pesquisa simples

Retorna os registros A e AAAA associados a um domínio

`nslookup example.com`

## Especificar um tipo de registro

`nslookup -type=A example.com`

## Especificar um servidor de DNS

`nslookup example.com 8.8.8.8`

## Realizar uma busca reversa

`nslookup -type=PTR 0.2.0.192.in-addr.arpa`

## Iniciar modo interativo

`nslookup`

Ou:

`nslookup - 8.8.8.8`

## Comandos interativos

* `<host>`: Procurar informação sobre o `host` (domínio totalmente qualificado, IP ou um subdomínio a ser qualificado pela lista de busca)
* `<host> <servidor>`: Procurar informação sobre o `host` utilizando o `servidor` especificado.
* `server <domínio>`: Modificar o servidor padrão para `domínio`. Utiliza o servidor padrão atual para procurar informação sobre `domínio`.
* `lserver <domínio>`: O mesmo que o anterior, porém utiliza o servidor inicial para procurar informação sobre `domínio`.
* `set all`: Mostrar os valores das opções, bem como o servidor definido.
* `set port=<valor>`: Especificar a porta do servidor.
* `set ty[pe]=<valor>`: Especificar o tipo de registro a ser consultado.
* `set domain=<domínio>`:  Definir a lista de busca, utilizada quando `host` não é um domínio completo.
* `exit`: Sair do programa.

Para mais opções, ver `man nslookup`.
