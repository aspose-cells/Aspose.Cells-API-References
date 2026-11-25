---
title: "LineFormat.CapType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LineFormat. Specifica i cappucci finali"
type: docs
url: /it/net/aspose.cells.drawing/lineformat/captype/
---
## LineFormat.CapType property

Specifica i cappucci finali.

```csharp
public LineCapType CapType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Imposta le proprietà del formato linea
            LineFormat lineFmt = line.Line;
            lineFmt.CapType = LineCapType.Flat;

            // Salva la cartella di lavoro
            workbook.Save("LineFormatCapTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LineCapType](../../linecaptype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


