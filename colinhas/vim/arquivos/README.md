# Vim - Arquivos

## Abrir

| Comando            | Função                                                                                           |
| ------------------ | ------------------------------------------------------------------------------------------------ |
| `:vi <arquivo>`    | abrir aquivo (funciona desde que o arquivo atual não tenha modificações não salvas)              |
| `:e <arquivo>`     | (o mesmo)                                                                                        |
| `:vi! <arquivo>`   | forçar abrir (fecha o arquivo atual e descarta as alteraç ões)                                   |
| `:e! <arquivo>`    | (o mesmo)                                                                                        |
| `:view  <arquivo>` | abrir como somente leitura (o mesmo que o comando `vi`, mas abre o arquivo como somente leitura) |
| `:read <arquivo>`  | ler arquivo e inserir seu conteúdo após a linha atual                                            |

## Salvar

Comandos:

| Comando             | Função                                                                                                   |
| ------------------- | -------------------------------------------------------------------------------------------------------- |
| `:write`            | salvar                                                                                                   |
| `:w`                | (o mesmo)                                                                                                |
| `:write!`           | forçar salvar (força o salvamento de arquivo aberto como somente leitura)                                |
| `:w!`               | (o mesmo)                                                                                                |
| `:write <arquivo>`  | salvar como outro arquivo                                                                                |
| `:w <arquivo>`      | (o mesmo)                                                                                                |
| `:write! <arquivo>` | forçar salvar como (sobrescreve o arquivo atual)                                                         |
| `:w! <arquivo>`     | forçar salvar como (sobrescreve o arquivo atual)                                                         |
| `:preserve`         | salvar temporariamente (salva no swap, o arquivo é mantido até ser executado algum comando para salvar)  |
| `:wq`               | salvar e sair                                                                                            |

Atalhos:

| Atalho            | Função                                     |
| ----------------- | ------------------------------------------ |
| <kbd>ZZ</kbd>     | o mesmo que o comando `wq` (salvar e sair) | 
