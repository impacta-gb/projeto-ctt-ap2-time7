Go possui estruturas poderosas para manipulação de dados 

--- 

# Array 

```go
var numeros [3]int

numeros[0] = 10
numeros[1] = 20
numeros[2] = 30 
```

---
# Slice 

```go 
nomes :=[]string{"marcos", "joão", "Maria"}
```

---

# Adicionando no Slice 

```go
nomes = append(nomes, "carlos")
```

---

#maps

```go 
idades :=map[string]int{
    "marcos": 25,
    "joão: 30,"

}
```

---

# Exemplo Completo 

```go
package "fmt"

func main(){
    
    frutas :=[]string{"Maçã", "Banana "}

    for -, frutas := range frutas {
        fmt.println(fruta)
    }
}
```

---

!!! note 
           Slice são muitos utilizados em Go por srem dinâmicos. 