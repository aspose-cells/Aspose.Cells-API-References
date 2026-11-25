---
title: "MsoLineFormat.Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormat. Restituisce un oggetto Style che rappresenta lo stile dell'intervallo specificato"
type: docs
url: /it/net/aspose.cells.drawing/msolineformat/style/
---
## MsoLineFormat.Style property

Restituisce un oggetto Style che rappresenta lo stile dell'intervallo specificato.

```csharp
public MsoLineStyle Style { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma linea
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);

            // Ottieni il formato della linea
            MsoLineFormat lineFormat = line.LineFormat;

            // Imposta le proprietà dello stile della linea
            lineFormat.Style = MsoLineStyle.ThickBetweenThin;
            lineFormat.ForeColor = System.Drawing.Color.Red;
            lineFormat.BackColor = System.Drawing.Color.White;
            lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 3.0;

            // Crea un'altra linea per confronto
            Aspose.Cells.Drawing.LineShape line2 = worksheet.Shapes.AddLine(5, 25, 100, 150, 10, 10);
            MsoLineFormat lineFormat2 = line2.LineFormat;

            // Copia lo stile dalla prima linea alla seconda linea
            lineFormat2.Style = lineFormat.Style;
            lineFormat2.ForeColor = lineFormat.ForeColor;
            lineFormat2.BackColor = lineFormat.BackColor;
            lineFormat2.DashStyle = lineFormat.DashStyle;
            lineFormat2.Transparency = lineFormat.Transparency;
            lineFormat2.Weight = lineFormat.Weight;

            // Salva la cartella di lavoro
            workbook.Save("MsoLineFormatStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


