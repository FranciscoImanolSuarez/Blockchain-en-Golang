## Blockchain en Go

Es un blockchain escrito en Go en menos de 200 lineas, la idea parte de la publicacion creada por [Coral Health](https://medium.com/@mycoralhealth) en Medium.

Este ejemplo fue basado en los latidos del corazón en reposo, en el tutorial nos explican como crear nuestro propio Blockchain, como escribir nuevos bloques, asi como tambien agregar los identificadores(SHA256).

`main.go`

Programa principal asi como tambien toda la lógica del Blockchain

`.env`

PORT=8080

#### Paso 1:

```git
git clone https://github.com/FranciscoImanolSuarez/Blockchain-en-Golang
```

#### Paso 2:

```go
go get github.com/davecgh/go-spew/spew
```

*Spew* nos permite ver `structs`y `slices`formatear limpiamente en nuestra consola.

```go
go get github.com/gorilla/mux
```

Gorilla / mux* es un paquete popular para escribir manejadores web. Vamos a necesitar esto.

```go
go get github.com/joho/godotenv
```

*Godotenv* nos permite leer un  `.env` archivo que guardamos en la raíz de nuestro directorio para que no tengamos que codificar cosas como nuestros puertos http.

#### Paso 3:

```go
go run main.go
```

Y deberiamos ver algo parecido a lo siguiente

![](https://github.com/FranciscoImanolSuarez/Blockchain-en-Golang/blob/master/.readme-static/Captura%20de%20pantalla%202019-01-19%20a%20la(s)%2018.31.55.png)

Asi como tambien podemos ir a localhost:8080

Para agregar bloques usaremos Postman como se ve en la siguiente imagen

![](https://cdn-images-1.medium.com/max/800/1*eYfFp1lqJUiAS1S6K8ZHbQ.png)

Luego refrescamos en localhost y podremos ver los nuevos bloques
