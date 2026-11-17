---
title: "Clase ProtectedRange"
linktitle: "ProtectedRange"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase ProtectedRange. Encapsula el objeto que representa protectedrange en Go."
type: docs
weight: 200
url: /es/go-cpp/protectedrange/
---

## ProtectedRange class

A specified range to be allowed to edit when the sheet protection is ON.

```go

type ProtectedRange struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetName](./getname/) | Obtiene el título del rango. Se usa como descriptor, no como una definición de rango con nombre. |
| [SetName](./setname/) | Obtiene el título del rango. Se usa como descriptor, no como una definición de rango con nombre. |
| [GetCellArea](./getcellarea/) | Obtiene el objeto CellArea que representa el área de celdas a proteger. |
| [GetAreas](./getareas/) | Obtiene todas las áreas referidas. |
| [AddArea](./addarea/) | Agrega un área referida a este. |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Indica si las hojas de cálculo están protegidas con contraseña. |
| [GetPassword](./getpassword/) | Representa la contraseña para proteger el rango. |
| [SetPassword](./setpassword/) | Representa la contraseña para proteger el rango. |
| [GetSecurityDescriptor](./getsecuritydescriptor/) | El descriptor de seguridad define las cuentas de usuario que pueden editar este rango sin proporcionar una contraseña para acceder al rango. |
| [SetSecurityDescriptor](./setsecuritydescriptor/) | El descriptor de seguridad define las cuentas de usuario que pueden editar este rango sin proporcionar una contraseña para acceder al rango. |
