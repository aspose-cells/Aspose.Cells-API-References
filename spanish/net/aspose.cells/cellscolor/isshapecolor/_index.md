---
title: "CellsColor.IsShapeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsColor. Obtiene y establece el color que debe aplicarse a la celda o forma"
type: docs
url: /es/net/aspose.cells/cellscolor/isshapecolor/
---
## CellsColor.IsShapeColor property

Obtiene y establece el color que debe aplicarse a la celda o forma.

```csharp
public bool IsShapeColor { get; set; }
```

### Observaciones

La expresión del color de la celda y la forma es diferente. Por ejemplo: el color de tema con el mismo valor de tono no será el mismo en la celda y la forma.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyIsShapeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de CellsColor y establecer IsShapeColor
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.IsShapeColor = true;
            cellsColor.Color = Color.Green;

            // Aplicar el color a una forma
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = cellsColor.Color;  // Use the Color property instead of CellsColor directly

            // Guarda el libro de trabajo
            workbook.Save("CellsColorIsShapeColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


