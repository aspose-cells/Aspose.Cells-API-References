---
title: "ShapeCollection.AddSpinner"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade un Spinner a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addspinner/
---
## ShapeCollection.AddSpinner method

Agrega un Spinner a la hoja de cálculo.

```csharp
public Spinner AddSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical del Spinner desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal del Spinner desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura del Spinner, en unidades de píxel. |
| ancho | Int32 | Representa el ancho del Spinner, en unidades de píxel. |

### Valor de retorno

Un objeto Spinner.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSpinnerWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añadir un spinner a la hoja de cálculo
            Aspose.Cells.Drawing.Spinner spinner = (Aspose.Cells.Drawing.Spinner)worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 50);

            // Establecer propiedades del spinner
            spinner.LinkedCell = "A1";
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 1;

            // Guarda el libro de trabajo
            workbook.Save("AddSpinnerDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Spinner](../../spinner/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


