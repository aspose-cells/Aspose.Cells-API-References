---
title: AddSpinner
second_title: Referencia de API de Aspose.Cells para .NET
description: Agrega un Spinner a la hoja de trabajo.
type: docs
weight: 290
url: /es/net/aspose.cells.drawing/shapecollection/addspinner/
---
## ShapeCollection.AddSpinner method

Agrega un Spinner a la hoja de trabajo.

```csharp
public Spinner AddSpinner(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| upperLeftRow | Int32 | Índice de la fila superior izquierda. |
| top | Int32 | Representa el desplazamiento vertical de Spinner desde su fila izquierda, en unidades de píxel. |
| upperLeftColumn | Int32 | Índice de la columna superior izquierda. |
| left | Int32 | Representa el desplazamiento horizontal de Spinner desde su columna izquierda, en unidades de píxel. |
| height | Int32 | Representa la altura de Spinner, en unidades de píxel. |
| width | Int32 | Representa el ancho de Spinner, en unidades de píxel. |

### Valor_devuelto

Un objeto Spinner.

### Ejemplos

```csharp

[C#]
//agregar una ruleta
Spinner spinner = shapes.AddSpinner(1, 0, 1, 0, 100, 50);
```

### Ver también

* class [Spinner](../../spinner)
* class [ShapeCollection](../../shapecollection)
* espacio de nombres [Aspose.Cells.Drawing](../../shapecollection)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
