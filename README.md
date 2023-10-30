# Saludos en Go

Este paquete proporciona una forma simple de obtener saludos personalizados en Go

## Instalacion
Ejecuta el siguiente comando para instalar el paquete:
```bash
go get -u github.com/lann892/greetings
```

## Uso
Aqui tienes un ejemplo de como utilizar el paquete con tu codigo:

```go
package main

import (
    "fmt"
    "github.com/lann892/greetings"
)

func main() {
    message, err := greetings.Hello("Lan")

    if err != nil {
        fmt.Println("Ocurrio un error:", err)
        return
    }

    fmt.Println(message)
}
```

Este ejemplo importa el paquete github.com/lann892/greetings y llama la funcion Hello que implementa un saludo personalizado. Si ocurre un error, se imprime un mensaje de error.
