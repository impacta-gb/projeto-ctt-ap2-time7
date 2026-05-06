# Gerenciamento de Pacotes (Go Modules)

Go Modules são o sistema oficial de gerenciamento de dependências da linguagem Go.

## Inicializando um projeto

```bash
go mod init meu-projeto
```

Esse comando cria o arquivo `go.mod`.

## Instalando dependências

```bash
go mod tidy
```

O comando remove dependências não utilizadas e instala as necessárias.

## Exemplo de go.mod

```go
module meu-projeto

go 1.22
```

## Principais comandos

| Comando | Função |
|---|---|
| go mod init | Inicializa projeto |
| go mod tidy | Organiza dependências |
| go run | Executa aplicação |
| go build | Gera executável |

!!! tip "Boa prática"
    Sempre execute `go mod tidy` antes de enviar o projeto.