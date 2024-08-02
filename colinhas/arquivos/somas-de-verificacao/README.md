# Somas de Verificação

## md5sum e shasum (coreutils)

### Calcular a soma de verificação MD5

`md5sum hello.txt > hello.txt.md5`

### Calcular a soma de verificação SHA1

`shasum hello.txt > hello.txt.sha1`

Ou:

`sha1sum hello.txt > hello.txt.sha1`

### Calcular a soma de verificação SHA256

`shasum --algorithm 256 hello.txt > hello.txt.sha256`

Ou:

`sha256sum hello.txt > hello.txt.sha256`

### Checar a soma de verificação (`--check` ou `-c`)

`md5sum -c hello.txt.md5`

### Algoritmos Suportados

* SHA1
* SHA224
* SHA256
* SHA384
* SHA512

### Outras Opções

* `--quiet`: exibe mensagem apenas no caso de arquivos ausentes ou falhas na verificação
* `--ignore-missing`: ignora arquivos ausentes
* `--status`: não exibe mensagens de sucesso ou falha, o código de saída indica o resultado

## openssl

### Listar algoritmos disponíveis

`openssl list -digest-algorithms`

### Calcular soma de verificação

`openssl dgst -sha3-512 hello.txt`

## rhash

### Listar algoritmos disponíveis

`rhash --list-hashes`

### Calcular soma de verificação

`rhash --sha3-512 hello.txt -o hello.txt.sha`

### Checar soma de verificação

`rhash -c hello.txt.sha`

### Ignorar arquivos ausentes e verificações bem sucedidas

`rhash -c --skip-ok --ignore-missing hello.txt.sha`
