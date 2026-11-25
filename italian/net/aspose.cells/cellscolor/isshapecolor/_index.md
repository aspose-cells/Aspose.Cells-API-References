---
title: "CellsColor.IsShapeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsColor. Ottiene e imposta il colore da applicare alla cella o alla forma"
type: docs
url: /it/net/aspose.cells/cellscolor/isshapecolor/
---
## CellsColor.IsShapeColor property

Ottiene e imposta il colore da applicare alla cella o alla forma.

```csharp
public bool IsShapeColor { get; set; }
```

### Osservazioni

L'espressione del colore della cella e della forma è diversa. Per esempio: il colore del tema con lo stesso valore di tinta non sarà lo stesso nella cella e nella forma.

### Esempi

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

            // Crea un'istanza di CellsColor e imposta IsShapeColor
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.IsShapeColor = true;
            cellsColor.Color = Color.Green;

            // Applica il colore a una forma
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = cellsColor.Color;  // Use the Color property instead of CellsColor directly

            // Salva la cartella di lavoro
            workbook.Save("CellsColorIsShapeColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


