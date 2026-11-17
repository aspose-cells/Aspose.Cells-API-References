---
title: "Clase ReferredArea"
linktitle: "ReferredArea"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase ReferredArea. Encapsula el objeto que representa referredarea en Go."
type: docs
weight: 200
url: /es/go-cpp/referredarea/
---

## ReferredArea class

Represents a referred area by the formula.

```go

type ReferredArea struct  {
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
| [IsExternalLink](./isexternallink/) | Indica si esto es un enlace externo. |
| [GetExternalFileName](./getexternalfilename/) | Obtén el nombre del archivo externo si esto es una referencia externa. |
| [GetSheetName](./getsheetname/) | Indica en qué hoja se encuentra esta referencia. |
| [GetSheetNames](./getsheetnames/) | Nombres de todas las hojas de cálculo a las que esta instancia hace referencia. |
| [IsEntireRow](./isentirerow/) | Indica si esta área contiene todas las columnas (fila completa). |
| [IsEntireColumn](./isentirecolumn/) | Indica si esta área contiene todas las filas (columna completa). |
| [IsArea](./isarea/) | Indica si esto es un área. |
| [GetEndColumn](./getendcolumn/) | La columna final del área. |
| [GetStartColumn](./getstartcolumn/) | La columna inicial del área. |
| [GetEndRow](./getendrow/) | La fila final del área. |
| [GetStartRow](./getstartrow/) | La fila inicial del área. |
| [GetValues](./getvalues/) | Obtiene los valores de celda en esta área. |
| [GetValues_Bool](./getvalues_bool/) | Obtiene los valores de celda en esta área. |
| [GetValue_Int_Int](./getvalue_int_int/) | Obtiene el valor de celda con el desplazamiento dado desde la esquina superior izquierda de esta área. |
| [GetValue_Int_Int_Bool](./getvalue_int_int_bool/) | Obtiene el valor de celda con el desplazamiento dado desde la esquina superior izquierda de esta área. |
| [ToString](./tostring/) | Devuelve la dirección de referencia de esta área. Generalmente es la dirección de la referencia que puede usarse en una fórmula, como "Sheet1!A1:C3". |
