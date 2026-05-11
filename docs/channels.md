# Concorrência II: Channels

Channels são utilizados em Go para permitir comunicação segura entre Goroutines.

## O que são Channels?

Um Channel permite enviar e receber dados entre diferentes Goroutines.

!!! info "Importante"
    Channels ajudam a evitar problemas de concorrência e compartilhamento de memória.

## Criando um Channel

```go
package main

import "fmt"

func main() {
    mensagens := make(chan string)

    go func() {
        mensagens <- "Olá do Channel!"
    }()

    msg := <-mensagens
    fmt.Println(msg)
}
```

## Channels Bufferizados

```go
package main

import "fmt"

func main() {
    canal := make(chan int, 2)

    canal <- 10
    canal <- 20

    fmt.Println(<-canal)
    fmt.Println(<-canal)
}
```

## Vantagens dos Channels

| Vantagem | Descrição |
|---|---|
| Segurança | Evita conflitos entre Goroutines |
| Organização | Facilita comunicação |
| Concorrência | Permite execução paralela |

!!! warning "Cuidado"
    Um channel sem leitura pode causar deadlock.