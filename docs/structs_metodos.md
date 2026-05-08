# Structs e Métodos em Go

## O que são Structs?

Structs em Go são estruturas utilizadas para agrupar diferentes tipos de dados em um único objeto.

Elas ajudam na organização e modelagem de informações.

### Exemplo de Struct

```go
package main

import "fmt"

type Pessoa struct {
    Nome  string
    Idade int
}

func main() {
    p := Pessoa{
        Nome:  "Luis",
        Idade: 20,
    }

    fmt.Println(p.Nome)
    fmt.Println(p.Idade)
}
```


# O que são métodos?

Métodos são funções associadas a uma struct.

Eles permitem adicionar comportamentos aos dados.

Exemplo de método:

```go

package main

import "fmt"

type Pessoa struct {
    Nome string
}

func (p Pessoa) Saudacao() {
    fmt.Println("Olá,", p.Nome)
}

func main() {
    pessoa := Pessoa{Nome: "Luis"}
    pessoa.Saudacao()
}
```

## Vantagens 

Melhor organização do código
Reutilização de estruturas
Encapsulamento de comportamento
Código mais limpo e legível 

