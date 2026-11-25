---
title: "Class MsoLineFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.MsoLineFormat class. Rappresenta la formattazione di linee e punte di freccia"
type: docs
url: /it/net/aspose.cells.drawing/msolineformat/
---
## MsoLineFormat class

Rappresenta la formattazione di linee e punte di freccia.

```csharp
public class MsoLineFormat
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformat/backcolor/) { get; set; } | Ottiene e imposta il colore di sfondo della linea del bordo. |
| [DashStyle](../../aspose.cells.drawing/msolineformat/dashstyle/) { get; set; } | Ottiene o imposta lo stile di tratteggio per la linea specificata. |
| [ForeColor](../../aspose.cells.drawing/msolineformat/forecolor/) { get; set; } | Ottiene e imposta il colore di primo piano della linea del bordo. |
| [IsVisible](../../aspose.cells.drawing/msolineformat/isvisible/) { get; set; } | Indica se l'oggetto è visibile. |
| [Style](../../aspose.cells.drawing/msolineformat/style/) { get; set; } | Restituisce un oggetto Style che rappresenta lo stile dell'intervallo specificato. |
| [Transparency](../../aspose.cells.drawing/msolineformat/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0.0 (opaco) a 1.0 (trasparente). |
| [Weight](../../aspose.cells.drawing/msolineformat/weight/) { get; set; } | Restituisce o imposta lo spessore della linea, in unità di pt. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatDemo
    {
        public static void MsoLineFormatExample()
        {
            // Istanzia un nuovo Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma ad arco al foglio di lavoro
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Ottieni l'oggetto MsoLineFormat dalla forma
            MsoLineFormat lineFormat = arcShape.LineFormat;

            // Imposta le proprietà dell'oggetto MsoLineFormat
            lineFormat.IsVisible = true;
            lineFormat.Style = MsoLineStyle.ThickThin;
            lineFormat.ForeColor = Color.Red;
            lineFormat.BackColor = Color.Blue;
            lineFormat.DashStyle = MsoLineDashStyle.Solid;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 2.0;

            // Salva la cartella di lavoro
            workbook.Save("MsoLineFormatExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


