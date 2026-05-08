# Tratamento de Erros (`tratamento_erros.md`)

# Tratamento de Erros em Go

## Introdução

Go utiliza um modelo simples e explícito para tratamento de erros.

O padrão mais utilizado é:

```go
if err != nil
```

### Exemplo Básico

```go

package main

import (
    "fmt"
    "os"
)

func main() {
    arquivo, err := os.Open("teste.txt")

    if err != nil {
        fmt.Println("Erro ao abrir arquivo:", err)
        return
    }

    defer arquivo.Close()

    fmt.Println("Arquivo aberto com sucesso!")
}
```

# Como Funciona?

Funções podem retornar um valor de erro (error)
Se ocorrer algum problema, err será diferente de nil
Caso contrário, err será nil

## Vantagens do Modelo

Código explícito
Fácil identificação de falhas
Evita exceções escondidas
Melhor controle do fluxo do programa

### Boas práticas

Sempre verificar erros retornados
Utilizar mensagens claras
Retornas erros quando necessário

