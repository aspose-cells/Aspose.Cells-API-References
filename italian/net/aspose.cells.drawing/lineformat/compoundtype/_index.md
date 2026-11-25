---
title: "LineFormat.CompoundType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LineFormat. Specifica il tipo di composto della linea"
type: docs
url: /it/net/aspose.cells.drawing/lineformat/compoundtype/
---
## LineFormat.CompoundType property

Specifica il tipo di composto della linea.

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCompoundTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Ottieni il formato della linea
            LineFormat lineFmt = line.Line;

            // Imposta tipo composto
            lineFmt.CompoundType = MsoLineStyle.Single;

            // Salva la cartella di lavoro
            workbook.Save("LineFormatCompoundTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoLineStyle](../../msolinestyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


