---
title: "LineFormat.EndArrowheadWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LineFormat. Ottiene e imposta il tipo di larghezza della freccia finale della linea"
type: docs
url: /it/net/aspose.cells.drawing/lineformat/endarrowheadwidth/
---
## LineFormat.EndArrowheadWidth property

Ottiene e imposta il tipo di larghezza della freccia finale della linea.

```csharp
public MsoArrowheadWidth EndArrowheadWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea
            Shape line = worksheet.Shapes.AddLine(10, 10, 100, 10, 5, 5);

            // Ottieni il formato della linea
            LineFormat lineFmt = line.Line;

            // Imposta la larghezza della freccia finale
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Salva la cartella di lavoro
            workbook.Save("LineFormatPropertyEndArrowheadWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


