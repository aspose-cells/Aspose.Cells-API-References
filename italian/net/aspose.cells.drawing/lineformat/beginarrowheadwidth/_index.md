---
title: "LineFormat.BeginArrowheadWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LineFormat. Ottiene e imposta il tipo di larghezza della freccia iniziale della linea"
type: docs
url: /it/net/aspose.cells.drawing/lineformat/beginarrowheadwidth/
---
## LineFormat.BeginArrowheadWidth property

Ottiene e imposta il tipo di larghezza della freccia iniziale della linea.

```csharp
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Imposta le proprietà del formato linea
            LineFormat lineFmt = line.Line;
            lineFmt.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Salva la cartella di lavoro
            workbook.Save("LineFormatDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


