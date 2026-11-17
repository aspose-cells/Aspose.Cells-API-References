---
title: "Clase Row"
linktitle: "Row"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase Row. Encapsula el objeto que representa row en Go."
type: docs
weight: 200
url: /es/go-cpp/row/
---

## Row class

Represents a single row in a worksheet.

```go

type Row struct  {
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
| [GetCellByIndex](./getcellbyindex/) | Obtén la celda por índice específico en la colección de celdas de este row. |
| [IsBlank](./isblank/) | Indica si el row contiene datos |
| [Get](./get/) | Obtiene la celda. |
| [GetEnumerator](./getenumerator/) | Obtiene el enumerador de celdas |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Obtiene un enumerador que itera celdas a través de este row. |
| [GetCellOrNull](./getcellornull/) | Obtiene la celda o null en el índice específico. |
| [IsCollapsed](./iscollapsed/) | si el row está colapsado |
| [SetIsCollapsed](./setiscollapsed/) | si el row está colapsado |
| [GetHeight](./getheight/) | Obtiene y establece la altura del row en unidades de Puntos. |
| [SetHeight](./setheight/) | Obtiene y establece la altura del row en unidades de Puntos. |
| [IsHidden](./ishidden/) | Indica si el row está oculto. |
| [SetIsHidden](./setishidden/) | Indica si el row está oculto. |
| [GetIndex](./getindex/) | Obtiene el índice de esta fila. |
| [GetGroupLevel](./getgrouplevel/) | Obtiene el nivel de grupo de la fila. |
| [SetGroupLevel](./setgrouplevel/) | Obtiene el nivel de grupo de la fila. |
| [IsHeightMatched](./isheightmatched/) | Indica si la altura de la fila coincide con la configuración de fuente predeterminada actual del libro. El valor verdadero de esta propiedad también indica que la altura de la fila es "automática" sin que el usuario haya establecido un valor de altura personalizado. |
| [SetIsHeightMatched](./setisheightmatched/) | Indica si la altura de la fila coincide con la configuración de fuente predeterminada actual del libro. El valor verdadero de esta propiedad también indica que la altura de la fila es "automática" sin que el usuario haya establecido un valor de altura personalizado. |
| [GetStyle](./getstyle/) | Obtiene el estilo de esta fila. |
| [SetStyle](./setstyle/) | Establece el estilo de esta fila. |
| [GetHasCustomStyle](./gethascustomstyle/) | Indica si esta fila tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada del libro). |
| [CopySettings](./copysettings/) | Copia la configuración de la fila, como estilo, altura, visibilidad, ...etc. |
| [GetFirstCell](./getfirstcell/) | Obtiene el primer objeto de celda en la fila. |
| [GetFirstDataCell](./getfirstdatacell/) | Obtiene la primera celda no vacía en la fila. |
| [GetLastCell](./getlastcell/) | Obtiene el último objeto de celda en la fila. |
| [GetLastDataCell](./getlastdatacell/) | Obtiene la última celda no vacía en la fila. |
| [ApplyStyle](./applystyle/) | Applies formats for a whole row. |
| [Equals_Object](./equals_object/) | Comprueba si este objeto se refiere a la misma fila que otro. |
| [Equals_Row](./equals_row/) | Comprueba si este objeto se refiere a la misma fila que otro objeto de fila. |
