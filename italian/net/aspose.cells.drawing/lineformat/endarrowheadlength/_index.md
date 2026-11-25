---
title: "LineFormat.EndArrowheadLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LineFormat. Ottiene e imposta il tipo di lunghezza della freccia finale della linea"
type: docs
url: /it/net/aspose.cells.drawing/lineformat/endarrowheadlength/
---
## LineFormat.EndArrowheadLength property

Ottiene e imposta il tipo di lunghezza della freccia finale della linea.

```csharp
public MsoArrowheadLength EndArrowheadLength { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea e ottieni direttamente l'oggetto forma
            LineShape line = (LineShape)worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Imposta la lunghezza della freccia finale
            line.Line.EndArrowheadLength = MsoArrowheadLength.Long;

            // Salva la cartella di lavoro
            workbook.Save("LineFormatPropertyEndArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


