# Testes Automatizados em Go

Go possui suporte nativo para testes automatizados através do pacote `testing`.

## Criando um teste

Arquivo:

```text
soma_test.go
```

## Exemplo

```go
package main

import "testing"

func Soma(a int, b int) int {
    return a + b
}

func TestSoma(t *testing.T) {
    resultado := Soma(2, 3)

    if resultado != 5 {
        t.Errorf("Esperado 5, recebido %d", resultado)
    }
}
```

## Executando testes

```bash
go test
```

## Benefícios dos testes

- Detectar erros rapidamente
- Garantir qualidade
- Facilitar manutenção

!!! success "Dica"
    Testes automatizados são essenciais em projetos profissionais.