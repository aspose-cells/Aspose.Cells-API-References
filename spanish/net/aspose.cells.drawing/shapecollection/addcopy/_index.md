---
title: "ShapeCollection.AddCopy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ShapeCollection método. Añade y copia una forma a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addcopy/
---
## AddCopy(Shape, int, int, int, int) {#addcopy}

Agrega y copia una forma a la hoja de cálculo.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceShape | Forma | Forma de origen. |
| topRow | Int32 | El índice de la fila superior. |
| superior | Int32 | Representa el desplazamiento vertical desde su fila superior, en unidades de píxel. |
| leftColumn | Int32 | El índice de la columna izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal desde su columna izquierda, en unidades de píxel. |

### Valor de retorno

El nuevo objeto [`Shape`](../../shape/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCopyWithShapeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar una forma rectangular
            RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Agregar una copia de la forma de rectángulo con nueva posición
            shapes.AddCopy(rectangle, 7, 0, 7, 0);

            // Guarda el libro de trabajo
            workbook.Save("ShapeCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Shape, int, int, int, int, CopyOptions) {#addcopy_1}

Agrega y copia una forma a la hoja de cálculo.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, 
    CopyOptions copyOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceShape | Forma | Forma de origen. |
| topRow | Int32 | El índice de la fila superior. |
| superior | Int32 | Representa el desplazamiento vertical desde su fila superior, en unidades de píxel. |
| leftColumn | Int32 | El índice de la columna izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal desde su columna izquierda, en unidades de píxel. |
| copyOptions | CopyOptions | Las opciones de copiar formas. |

### Valor de retorno

El nuevo objeto [`Shape`](../../shape/).

### Ejemplos

```csharp

[C#]
//agregar una forma
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//Agrega y copia una forma.
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

### Ver también

* class [Shape](../../shape/)
* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


