# Estruturas de Controle

Go possui estruturas simples e eficientes para controle de fluxo.

---

# if

```go 
idade := 18

if idade >= 118{
    fmt.println("maior idade")
}
```

---

  # If/ Else

```go
if idade >= 18{
    fmt.println("maior")
} else {
    fmt.println("menor")
}
```

---

# For

```go
for i := 0; i < 5; i++ {
    fmt.println(i)
}
```

---

#loop Infinito 

```go
for {
    fmt.println("Executando...")
}
```

---

# Switch

```go
dia :=2

switch dia {
case 1:
    fmt.println("Domingo")

case 2:
    fmt.println("Segunda")


default:
    fmt.println("Outro dia")

}
```

---

!!! warnig
    Evite loops infitnitos sem condições de parada.



