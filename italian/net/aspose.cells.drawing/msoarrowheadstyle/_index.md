---
title: "Enum MsoArrowheadStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.MsoArrowheadStyle enum. Elenca i tipi di estremità della linea del bordo della forma"
type: docs
url: /it/net/aspose.cells.drawing/msoarrowheadstyle/
---
## MsoArrowheadStyle enumeration

Enumera il tipo di estremità della linea del bordo della forma.

```csharp
public enum MsoArrowheadStyle
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessun tipo di estremità della linea. |
| Arrow | `1` | Tipo di estremità a freccia. |
| ArrowStealth | `2` | Tipo di estremità a freccia stealth. |
| ArrowDiamond | `3` | Tipo di estremità a freccia diamante. |
| ArrowOval | `4` | Tipo di estremità a freccia ovale. |
| ArrowOpen | `5` | Tipo di estremità a freccia aperta. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassMsoArrowheadStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea
            LineShape lineShape = worksheet.Shapes.AddLine(5, 5, 10, 10, 100, 100);

            // Imposta le proprietà della linea
            MsoLineFormat lineFormat = lineShape.LineFormat;
            lineFormat.ForeColor = System.Drawing.Color.Black;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 0.75;

            // Imposta gli stili della punta della freccia
            lineShape.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
            lineShape.Line.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineShape.Line.BeginArrowheadLength = MsoArrowheadLength.Medium;
            lineShape.Line.EndArrowheadLength = MsoArrowheadLength.Medium;

            // Salva la cartella di lavoro
            workbook.Save("MsoArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


