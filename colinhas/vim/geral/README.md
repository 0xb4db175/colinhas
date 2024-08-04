# Vim - Geral

## Alternar Modos

### Modo Inserir

Inserção Simples:

| Comando | Função |
| ------- | ------ |
| `i` | Entrar em modo inserir antes do local atual do cursor | 
| `a` | Entrar em modo inserir após o local atual do cursor |
| `I` | Entrar em modo inserir no começo da linha atual |
| `gI` | Entrar em modo inserir na primeira coluna da linha atual |
| `A` | Entrar em modo inserir no final da linha atual |
| `o` | Entrar em modo inserir abrindo uma linha abaixo da linha atual |
| `O` | Entrar em modo inserir abrindo uma linha acima da linha atual |

Substituição e Inserção:

| Comando | Função |
| ------- | ------ |
| `s` | Entrar em modo inserir, eliminando o caractere atual |
| `c<m>` | Entrar em modo inserir, eliminando do cursor até o local correspondente ao movimento <m>(1) |
| `C` | Entrar em modo inserir, eliminando do cursor até o final da linha |
| `S` | Entrar em modo inserir, eliminando toda a linha atual |
| `cc` | (o mesmo) |

(1) - Para maiores informações, ver a seção **Movimentos**

### Modo Substituir

Ativa o cursor e inicia a substituição conforme os novos caracteres são digitados:

| Comando | Função |
| ------- | ------ |
| `R` | Entrar em modo substituir a partir do local atual do cursor |

### Modo Visual

| Comando | Função |
| ------- | ------ |
| `v` | Selecionar caracteres no modo visual |
| `SHIFT-v` | Selecionar linhas no modo visual |
| `CTRL-v` | Selecionar blocos no modo visual |

### Modo Normal

| Comando | Função |
| ------- | ------ |
| `<ESC>` | Retornar ao modo normal |

## Sair

| Comando | Função                                                |
| ------- | ----------------------------------------------------- |
| `:q`    | Sair                                                  |
| `:q!`   | Forçar saída (descarta alterações não salvas)         |
| `:qa`   | Sair de tudo                                          |
| `:qa!`  | Forçar saída de tudo (descarta alterações não salvas) |
