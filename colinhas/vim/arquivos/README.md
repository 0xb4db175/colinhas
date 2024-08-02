# Vim - Arquivos

## Abrir

| Comando      | Função                                                                                                |
| ------------ | ----------------------------------------------------------------------------------------------------- |
| `:vi <a>`    | abrir aquivo \<a> (funciona desde que o arquivo atual não tenha modificações não salvas)              |
| `:e <a>`     | (o mesmo)                                                                                             |
| `:vi! <a>`   | forçar abrir o arquivo \<a> (fecha o arquivo atual e descarta as alterações)                          |
| `:e! <a>`    | (o mesmo)                                                                                             |
| `:view  <a>` | abrir como somente leitura (o mesmo que o comando `vi`, mas abre o arquivo \<a> como somente leitura) |
| `:read <a>`  | ler arquivo \<a> e inserir seu conteúdo após a linha atual                                            |

## Salvar

Comandos:

| Comando       | Função                                                                                                   |
| ------------- | -------------------------------------------------------------------------------------------------------- |
| `:write`      | salvar                                                                                                   |
| `:w`          | (o mesmo)                                                                                                |
| `:write!`     | forçar salvar (força o salvamento de arquivo aberto como somente leitura)                                |
| `:w!`         | (o mesmo)                                                                                                |
| `:write <a>`  | salvar como arquivo \<a>                                                                                 |
| `:w <a>`      | (o mesmo)                                                                                                |
| `:write! <a>` | forçar salvar como \<a> (sobrescreve o arquivo atual)                                                    |
| `:w! <a>`     | (o mesmo)                                                                                                |
| `:preserve`   | salvar temporariamente (salva no swap, o arquivo é mantido até ser executado algum comando para salvar)  |
| `:wq`         | salvar e sair                                                                                            |

Atalhos:

| Atalho            | Função                                     |
| ----------------- | ------------------------------------------ |
| <kbd>ZZ</kbd>     | o mesmo que o comando `wq` (salvar e sair) | 
