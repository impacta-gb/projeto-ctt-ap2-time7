
# Concorrência com Goroutines (`goroutines.md`)

```markdown id="p4v8m6"
# Concorrência em Go com Goroutines

## O que são Goroutines?

Goroutines são funções executadas concorrentemente em Go.

Elas permitem que múltiplas tarefas sejam executadas ao mesmo tempo de forma leve e eficiente.

## Como Criar uma Goroutine

Utiliza-se a palavra-chave:

```go
go

# Exemplo Básico

package main

import (
    "fmt"
    "time"
)

func tarefa() {
    fmt.Println("Executando tarefa...")
}

func main() {
    go tarefa()

    time.Sleep(time.Second)
}

## Como Funciona?

A função tarefa() é executada concorrentemente
O programa principal continua executando sem esperar
time.Sleep() foi usado para dar tempo da goroutine finalizar

### Vantagens das Goroutines

Baixo consumo de memória
Alta performace
Facilidade para trabalhar com concorrência 
Simplicidade na criação de tarefas paralelas

## Casos de Uso 

Servidores Web 
Processamento paralelo
APIs
Operações em background

