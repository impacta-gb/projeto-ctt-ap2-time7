# Sintaxe basica e variáveis

Go é uma linguagem simples. rápida e fortemente tipada.

---

## Declarando Variáveis

```go 
var nome string = "marcos"
var idade int = 25
``` 

---

## Declaração Simplificada 
```go 
cidade := "São Paulo"
```

---

## Constantes 

```go 
cons PI = 3.14

---

## Tipos Básicos 
| tipo |Exemplo|
|------|--------|
| string| "texto" |
| int | 10 |
| float64 | 10.5 |
| bool | true |

---
!!! tip    
      Utilize `:=` para declarações rápidas dentro de funções.
    
---

##     Exmplo completo

```go 
packge main

import "fmt"

func main() {
    nome := "marcos"
    idade := 30

    fmt.println(nome)
    fmt.println(idade)
}
```
