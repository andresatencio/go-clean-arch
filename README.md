# go-clean-arch
Una traduccion del proyecto a Español

## Descripcion
Este es un ejemplo de implementacion de  Clean Architecture en proyectos Go (Golang).

Reglas de Clean Architecture by Uncle Bob
 * Independiente de frameworks. La arquitectura no depende de ninguna libreria. Esto permite usar los frameworks como herramientas y al revés.
 * Testeable. Las reglas de negocio deben permitirse verficiar sin hacer uso de UI, o base de datos o cualquier entidad externa.
 * Independiente de la UI. La UI puede cambiar facilmente sin que tenga que cambiar el sistema. La interfaz web podria cambia a una interfaz de terminal sin que esto implique cambiar las reglas de negocio.
 * Independiente de la base de datos.
 * Independiente de cualquier entidad externa. Las reglas de negocio no tienen porque conocerlas.

More at https://8thlight.com/blog/uncle-bob/2012/08/13/the-clean-architecture.html

Este proyecto tiene 4 capas de dominio :
 * Capa de Modelos
 * Capa de repositorios
 * Capa de casos de usos 
 * Capa de entrega

The explanation about this project's structure  can read from this medium's post : https://medium.com/@imantumorang/golang-clean-archithecture-efd6d7c43047

### How To Run This Project

```bash
#move to directory
cd $GOPATH/src/github.com/bxcodec

# Clone into YOUR $GOPATH/src
git clone https://github.com/bxcodec/go-clean-arch.git

#move to project
cd go-clean-arch

# Install Dependencies
dep ensure

# Make File
make

# Run Project
go run main.go

```

Or

```bash
# GET WITH GO GET
go get github.com/bxcodec/go-clean-arch

# Go to directory

cd $GOPATH/src/github.com/bxcodec/go-clean-arch

# Install Dependencies
dep ensure

# Make File
make

# Run Project
go run main.go
```


> Make Sure you have run the article.sql in your mysql

### Tools Used:
In this project, I use some tools listed below. But you can use any simmilar library that have the same purposes. But, well, different library will have different implementation type. Just be creative and use anything that you really need. 

- All libraries listed in [`Gopkg.toml`](https://github.com/bxcodec/go-clean-arch/blob/master/Gopkg.toml) 
- ["github.com/vektra/mockery".](https://github.com/vektra/mockery) To Generate Mocks for testing needs.


### Change log 
 - 2018-04-30 : [Move to new projects folder](https://github.com/bxcodec/go-clean-arch/pull/8)
 - 2018-05-09 : [Add Context](https://github.com/bxcodec/go-clean-arch/pull/9)
