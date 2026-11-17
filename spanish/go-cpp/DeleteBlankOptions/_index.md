---
title: "DeleteBlankOptions Clase"
linktitle: "DeleteBlankOptions"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "DeleteBlankOptions clase. Encapsula el objeto que representa deleteblankoptions en Go."
type: docs
weight: 200
url: /es/go-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

Represents the setting of deleting blank cells/rows/columns.

```go

type DeleteBlankOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewDeleteBlankOptions](./newdeleteblankoptions/) | Default constructor. |
| [NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | Constructs from a parent object. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetEmptyStringAsBlank](./getemptystringasblank/) | Indica si una celda se considerará vacía cuando su valor sea una cadena vacía.Valor predeterminado es verdadero. |
| [SetEmptyStringAsBlank](./setemptystringasblank/) | Indica si una celda se considerará vacía cuando su valor sea una cadena vacía.Valor predeterminado es verdadero. |
| [GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | Indica si una celda se considerará vacía cuando es una fórmula y el resultado calculado es nulo o una cadena vacía.Valor predeterminado es falso. |
| [SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | Indica si una celda se considerará vacía cuando es una fórmula y el resultado calculado es nulo o una cadena vacía.Valor predeterminado es falso. |
| [GetDrawingsAsBlank](./getdrawingsasblank/) | Indica si los objetos relacionados con dibujos, como imágenes, formas, gráficos..., se considerarán vacíos.Valor predeterminado es verdadero. |
| [SetDrawingsAsBlank](./setdrawingsasblank/) | Indica si los objetos relacionados con dibujos, como imágenes, formas, gráficos..., se considerarán vacíos.Valor predeterminado es verdadero. |
| [GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | Indica cómo procesar celdas combinadas al eliminar filas/columnas vacías. |
| [SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | Indica cómo procesar celdas combinadas al eliminar filas/columnas vacías. |
| [GetStartIndex](./getstartindex/) | Especifica el índice de fila/columna inicial del rango a comprobar y eliminar filas/columnas en blanco. |
| [SetStartIndex](./setstartindex/) | Especifica el índice de fila/columna inicial del rango a comprobar y eliminar filas/columnas en blanco. |
| [GetEndIndex](./getendindex/) | Especifica el índice de fila/columna final (inclusive) del rango a comprobar y eliminar filas/columnas en blanco. El valor predeterminado es -1 y -1 significa el rango máximo de todos los objetos (celdas, dibujos, ...) que deben comprobarse. |
| [SetEndIndex](./setendindex/) | Especifica el índice de fila/columna final (inclusive) del rango a comprobar y eliminar filas/columnas en blanco. El valor predeterminado es -1 y -1 significa el rango máximo de todos los objetos (celdas, dibujos, ...) que deben comprobarse. |
| [GetUpdateReference](./getupdatereference/) | Indicates if update references in other worksheets. |
| [SetUpdateReference](./setupdatereference/) | Indicates if update references in other worksheets. |
| [GetFormulaChangeMonitor](./getformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the deletion. |
| [SetFormulaChangeMonitor](./setformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the deletion. |
