---
title: "LineFormat.EndArrowheadStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LineFormat. Ottiene e imposta il tipo di freccia finale della linea"
type: docs
url: /it/net/aspose.cells.drawing/lineformat/endarrowheadstyle/
---
## LineFormat.EndArrowheadStyle property

Ottiene e imposta il tipo di freccia finale della linea.

```csharp
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Ottieni il formato della linea
            LineFormat lineFmt = line.Line;

            // Imposta lo stile della freccia finale
            lineFmt.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Salva la cartella di lavoro
            workbook.Save("LineFormatPropertyEndArrowheadStyleDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


