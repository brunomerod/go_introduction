# GO Hands On

## Dia 01

### Golang
* Go é uma linguagem de alto nível Garbage collected
* É rápida, intuitiva e fácil de utilizar

### Go vs Outras linguagens
* Go não possui operador ternário
* Go não possui list comprehenssion
* Go possui apenas uma forma de loop: **for**
* Go é uma linguagem com *tipagem* estática
* Go possui uma API de testes nativa

### Comandos fundamentais

1. Iniciar um novo projeto  
```
go mod init <nome do projeto>
```

2. Atualizar dependências  
```
go mod tidy
```

3. Rodar uma aplicação ou arquivo
```
# Roda aplicação e procura o package main
go run .

# Roda arquivo específico
go run file.go
```

4. Build -> criar binário da aplicação
```
go build -o <path/arquivo de output>
```

5. Build para outras plataformas é necessário alterar ou setar variável de ambiente  
GOOS = Go OS  
GOARCH = arquitetura da máquina
```
# Win
GOOS=windows GOARCH=386 go build -o binario.exe

# Linux
CGO_ENABLED=0 GOOS=linux GOARCH=amd64 go build -o binario
```

6. Adicionar lib ao projeto
```
go get <endereço da lib>
```

7. Instala um binário Go
```
go install <endereço da lib>
```

### Variáveis

### Funções

### Loop

### Struct

## Referências
Go PlayGround  
https://go.dev/play/

Standard lib  
https://pkg.go.dev/std

TDD With Go  
https://larien.gitbook.io/aprenda-go-com-testes/

