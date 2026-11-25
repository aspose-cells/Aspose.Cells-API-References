---
title: "LineFormat.BeginArrowheadStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LineFormat. Ottiene e imposta il tipo di freccia iniziale della linea"
type: docs
url: /it/net/aspose.cells.drawing/lineformat/beginarrowheadstyle/
---
## LineFormat.BeginArrowheadStyle property

Ottiene e imposta il tipo di freccia iniziale della linea.

```csharp
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Imposta lo stile della freccia iniziale
            line.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Salva la cartella di lavoro
            workbook.Save("LineFormatPropertyBeginArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


