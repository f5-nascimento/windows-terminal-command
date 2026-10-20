# windows-terminal-command

Este repositório reúne comandos úteis para navegação no sistema de arquivos, criação de diretórios, diagnóstico de redes, gerenciamento de processos e ferramentas de desenvolvimento. O objetivo é apoiar o aprendizado prático por meio de exemplos que podem ser executados no Prompt de Comando (CMD) e no PowerShell.

## Sumário

- [Navegação e Diretórios](#navegação-e-diretórios)
- [Diagnóstico de Rede](#diagnóstico-de-rede)
- [Gerenciamento de Processos](#gerenciamento-de-processos)
- [Ambiente de Desenvolvimento](#ambiente-de-desenvolvimento)
- [Registro de Sessão no PowerShell](#registro-de-sessão-no-powershell)

## Navegação e Diretórios

| Comando | Finalidade | Exemplo |
|---|---|---|
| `dir` | Lista os arquivos e diretórios do local atual. | `dir` |
| `cd` | Acessa outro diretório. | `cd Documentos` |
| `cd ..` | Retorna ao diretório anterior. | `cd ..` |
| `cd \` | Acessa a raiz da unidade atual. | `cd \` |
| `tree` | Exibe a estrutura de diretórios em formato de árvore. | `tree` |
| `mkdir` | Cria um novo diretório. | `mkdir Projeto` |

## Diagnóstico de Rede

| Comando | Finalidade | Exemplo |
|---|---|---|
| `hostname` | Exibe o nome do computador na rede. | `hostname` |
| `ipconfig` | Exibe informações básicas da configuração IP. | `ipconfig` |
| `ipconfig /all` | Exibe informações detalhadas da configuração de rede, incluindo servidores DNS. | `ipconfig /all` |
| `ping` | Testa a conectividade com um destino. | `ping globo.com` |
| `tracert` | Exibe os saltos percorridos pelos pacotes até um destino. | `tracert globo.com` |
| `netstat -ano` | Exibe conexões de rede, portas e identificadores dos processos (PID) associados. | `netstat -ano` |

## Gerenciamento de Processos

| Comando | Finalidade | Exemplo |
|---|---|---|
| `tasklist` | Lista os processos em execução. | `tasklist` |
| `taskkill` | Encerra um processo pelo nome ou pelo PID. | `taskkill /PID 1234 /T` |

> **Atenção:** substitua `1234` pelo PID de um processo apropriado para teste. Evite encerrar processos essenciais do sistema.

## Ambiente de Desenvolvimento

| Comando | Finalidade | Exemplo |
|---|---|---|
| `code .` | Abre o diretório atual no Visual Studio Code, desde que o comando esteja configurado. | `code .` |
| `--version` | Exibe a versão do Python disponível no terminal. | `python --version` |

## Registro de Sessão no PowerShell

O PowerShell permite registrar os comandos executados e suas respectivas saídas em um arquivo de texto.

| Comando | Finalidade | Exemplo |
|---|---|---|
| `Start-Transcript` | Inicia o registro da sessão do PowerShell em um arquivo. | `Start-Transcript -Path "$HOME\Projeto\Relatorio_CMD.txt"` |
| `Stop-Transcript` | Encerra o registro da sessão. | `Stop-Transcript` |

