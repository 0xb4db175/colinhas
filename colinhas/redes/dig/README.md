# dig

Comando `dig`.

## Obter o registro A associado a um domínio (apenas IP)

`dig +short example.com`

## Obter o registro A associado a um domínio (registro completo)

`dig +noall +answer example.com`

## Obter o registro A associado a um domínio (resposta detalhada)

`dig example.com`

## Obter um tipo específico de registro

`dig +short example.com AAAA`

Ou:

`dig +short -t AAAA example.com`

## Especificar um servidor de DNS

`dig +short @8.8.8.8 example.com`

## Realizar uma busca reversa

`dig -x 192.0.2.0`

## Principais flags

* `-4`: Usar apenas IPv4 no transporte da consulta.
* `-6`: Usar apenas IPv6 no transporte da consulta.
* `-f`: Especificar um arquivo contendo domínios a serem procurados.
* `-p`: Especificar a porta do servidor DNS.
* `-r`: **Não** ler configurações do arquivo `.digrc`.
* `-t`: Especificar o tipo de registro a ser consultado.
* `-x`: Efetuar busca reversa, mapeando endereços IP para nomes.

## Opções de exibição

* `+[no]all`: Desabilitar ou habilitar todas as opções de exibição.
* `+[no]comments`: Controlar a exibição de comentários.
* `+[no]cmd`: Controlar a exibição do comando.
* `+[no]edns`: Controlar a exibição da seção de EDNS.
* `+[no]question`: Controlar a exibição da seção de pergunta.
* `+[no]answer`: Controlar a exibição da seção de resposta.
* `+[no]authority`: Controlar a exibição da seção de autoridade.
* `+[no]stats`: Controlar a exibição da seção de estatísticas.
* `+short`: Exibir apenas a forma curta das respostas.
* `+trace`: Exibir o rastreamento desde os servidores raiz até o servidor de nome.
* `+yaml`: Exibir os resultados em formato YAML.
* `+domain=<domínio>`: Especificar um domínio padrão.

Para (muitas) outras opções, ver `dig -h` e `man dig`.

## Arquivo de configuração

`~/.digrc`

Exemplo:

```
+noall +answer
```
