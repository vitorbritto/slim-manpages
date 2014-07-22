# SLIM BASH

Um guia de bolso com informações extraídas do `man bash`.

## Tabela de Conteúdo

- [Sobre](#sobre)
- [Opções](#opções)
- [Argumentos](#argumentos)
- [Invocação](#invocação)
- [Definições](#definições)
- [Palavras reservadas](#palavras-reservadas)
- [Gramática do Shell](#gramática-do-shell)


## Sobre 

Bash é um interpretador capaz de executar comandos de leitura através de um arquivo ou do terminal (input) e incorpora recursos do Korn e C Shells (ksh e csh).

## Opcões

O Bash dispõe das seguintes opções:

| Flag (chave) | Descrição |
|--------------|-----------|
| -c | | 
| -i | | 
| -r | | 
| -s | | 
| -l, --login | | 
| -v, --verbose | | 
| -D, --dump-po-strings, --dump-strings | | 
| [-+]O | | 
| --debugger | | 
| --help | | 
| --init-file | | 
| --rcfile | | 
| --noediting | | 
| --noprofile | | 
| --norc | |
| --posix | |
| --restricted | |
| --version | |

## Argumentos

O primeiro arugmento do Bash é passado como `$0` o qual se refere ao nome do arquivo/programa em execução. O interpretador Bash faz uma primeira tentativa em abrir um arquivo no diretório corrente, se não encontrar fará uma busca nos diretórios adicionados na variável de ambiente PATH.

## Invocação

- Quando o Bash é invocado como um shell interativo (autenticado) ou como um shell interativo seguido da opção `--login`, o arquivo em `/etc/profile` será executado primeiramente. Após a leitura do arquivo, fará uma busca por `~/.bash_profile`, `~/.bash_login` e `~/.profile` nesta ordem. Executando os comandos no qual forem encontrados primeiro.
- Quando uma sessão shell (autenticada) é finalizada, o bash fará uma leitura do arquivo `~/bash_logout` e dos comandos existentes neste arquivo (caso existam).
- Quando uma sessão do shell (não autenticada) é iniciada, o bash fará a leitura dos comandos existentes no arquivo `~/.bashrc` (caso exista). Isto pode ser evitado com a opção `--norc`. A opção `--rcfile` vai forçar o bash a ler e executar os comandos do arquivo ao invés do `~/.bashrc`.

## Definições

- `blank`: 
- `word`:
- `name`:
- `metacharacter`:
- `control operator`: 

## Palavras reservadas

## Gramática do Shell

### Main

- Simples Commands
- Pipelines
- Lists
- Compound Commands
- Coprocesses
- Shell Function Definitions

### Comments

### Quoting

### Parameters

- Positional Parameters
- Special Parameters
- Shell Variables
- Arrays

### Expansion

- Brace Expansion
- Tilde Expansion
- Parameter Expansion
- Command Substitution
- Arithmetic Expansion
- Process Substitution
- Word Splitting
- Pathname Expansion
    - Pattern Matching
- Quote Removal 

### Redirection

- Redirecting Input
- Redirecting Output
- Appending Redirected Output
- Redirecting Standard Output and Standard Error
- Appending Standard Output and Standard Error
- Here Documents
- Here Strings
- Duplicating File Descriptors
- Moving File Descriptors
- Opening File Descriptors for Reading and Writing

### Aliases

### Functions

### Arithmetic Evaluation

### Conditional Expressions

### Simple Command Expansion

### Command Execution and Command Execution Environment

### Environment

### Exit Status

### Signals

     1) SIGHUP	  2) SIGINT	    3) SIGQUI    4) SIGILL
     5) SIGTRAP	  6) SIGABRT	    7) SIGEMT    8) SIGFPE
     9) SIGKILL	 10) SIGBUS	   11) SIGSEGV  12) SIGSYS
    13) SIGPIPE	 14) SIGALRM	   15) SIGTERM  16) SIGURG
    17) SIGSTOP	 18) SIGTSTP	   19) SIGCONT  20) SIGCHLD
    21) SIGTTIN	 22) SIGTTOU	   23) SIGIO    24) SIGXCPU
    25) SIGXFSZ	 26) SIGVTALRM  27) SIGPROF  28) SIGWINCH
    29) SIGINFO	 30) SIGUSR1	   31) SIGUSR2

### Job Control

### Prompting

### Readline

- Readline Notation
- Readline Initialization
- Readline Key Bindings
- Readline Variables
- Readline Conditional Constructs
- Searching
- Readline Command Names
- Commands for Moving
- Commands for Manipulating the History
- Commands for Changing Text
- Killing and Yanking
- Numeric Arguments
- Completing
- Keyboard Macros
- Miscellaneous
- Programmable Completion

### History and History Expansion

 - Event Designators
 - Word Designators
 - Modifiers

### Shell Builtin Commands

### Restricted Shell

### Files
