---
title: "LineFormat.BeginArrowheadLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LineFormat. Ottiene e imposta il tipo di lunghezza della freccia iniziale della linea"
type: docs
url: /it/net/aspose.cells.drawing/lineformat/beginarrowheadlength/
---
## LineFormat.BeginArrowheadLength property

Ottiene e imposta il tipo di lunghezza della freccia iniziale della linea.

```csharp
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea
            Shape lineShape = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
            LineShape line = (LineShape)lineShape;

            // Imposta la lunghezza della freccia iniziale
            line.Line.BeginArrowheadLength = MsoArrowheadLength.Long;

            // Salva la cartella di lavoro
            workbook.Save("LineFormatPropertyBeginArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


