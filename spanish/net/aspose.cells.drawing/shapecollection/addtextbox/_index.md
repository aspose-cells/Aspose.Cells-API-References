---
title: AddTextBox
second_title: Referencia de API de Aspose.Cells para .NET
description: Agrega un cuadro de texto a la hoja de cálculo.
type: docs
weight: 310
url: /es/net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

Agrega un cuadro de texto a la hoja de cálculo.

```csharp
public TextBox AddTextBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| upperLeftRow | Int32 | Índice de la fila superior izquierda. |
| top | Int32 | Representa el desplazamiento vertical del cuadro de texto desde su fila izquierda, en unidades de píxel. |
| upperLeftColumn | Int32 | Índice de la columna superior izquierda. |
| left | Int32 | Representa el desplazamiento horizontal del cuadro de texto desde su columna izquierda, en unidades de píxel. |
| height | Int32 | Representa la altura del cuadro de texto, en unidades de píxel. |
| width | Int32 | Representa el ancho del cuadro de texto, en unidades de píxel. |

### Valor_devuelto

A[`TextBox`](../../textbox) objeto.

### Ejemplos

```csharp

[C#]

//añadir un cuadro de texto
TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
```

### Ver también

* class [TextBox](../../textbox)
* class [ShapeCollection](../../shapecollection)
* espacio de nombres [Aspose.Cells.Drawing](../../shapecollection)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
