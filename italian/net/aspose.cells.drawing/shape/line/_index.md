---
title: "Shape.Line"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene lo stile della linea"
type: docs
url: /it/net/aspose.cells.drawing/shape/line/
---
## Shape.Line property

Ottiene lo stile della linea

```csharp
public LineFormat Line { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea (restituisce direttamente LineShape)
            LineShape lineShape = worksheet.Shapes.AddLine(1, 0, 1, 0, 5, 100);

            // Accedi e modifica le proprietà della linea
            LineFormat lineFormat = lineShape.Line;
            lineFormat.CompoundType = MsoLineStyle.ThickThin;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 3.0;
            lineFormat.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineFormat.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Salva la cartella di lavoro
            workbook.Save("LineShapeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [LineFormat](../../lineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


