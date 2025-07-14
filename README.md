# Seminario_Clientes

Proyecto de Java para el seminario. Incluye gestión de clientes, estructura modular y buenas prácticas.

## Compilar y ejecutar

```bash
javac src/Main.java
java Main


## Documentación

En la carpeta `docs/` están los archivos relacionados con la documentación del proyecto:

- `registro_interesados.xlsx`: Excel con el registro de interesados.
- `diagrama_uml.png`: Diagrama UML del proyecto.


## Funcionalidades posibles para el módulo Clientes:

Registrar cliente nuevo

Modificar datos del cliente

Consultar historial de cliente

Eliminar cliente

Buscar cliente por nombre o cédula




## Archivo .puml – Ejemplo para el módulo Clientes:
@startuml
title Diagrama de Casos de Uso - Módulo Clientes

actor "Empleado" as Emp
actor "Administrador" as Admin

rectangle "Sistema de Gestión de Clientes" {
  usecase "Registrar nuevo cliente" as UC1
  usecase "Modificar datos del cliente" as UC2
  usecase "Consultar historial del cliente" as UC3
  usecase "Eliminar cliente" as UC4
  usecase "Buscar cliente" as UC5
}

Emp --> UC1
Emp --> UC2
Emp --> UC3
Emp --> UC5
Admin --> UC4

@enduml

