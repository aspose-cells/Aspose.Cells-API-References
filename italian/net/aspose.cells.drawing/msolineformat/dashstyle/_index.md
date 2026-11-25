---
title: "MsoLineFormat.DashStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormat. Ottiene o imposta lo stile di tratteggio per la linea specificata"
type: docs
url: /it/net/aspose.cells.drawing/msolineformat/dashstyle/
---
## MsoLineFormat.DashStyle property

Ottiene o imposta lo stile di tratteggio per la linea specificata.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyDashStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi una forma per dimostrare DashStyle
            Shape shape = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Imposta le proprietà della linea
            shape.LineFormat.Style = MsoLineStyle.Single;
            shape.LineFormat.Weight = 3;
            shape.LineFormat.ForeColor = Color.Blue;

            // Dimostra diversi stili di tratteggio
            shape.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            shape.Text = "Solid Line";

            // Aggiungi un'altra forma con uno stile di tratteggio diverso
            Shape shape2 = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 3, 0, 200, 100);
            shape2.LineFormat.Style = MsoLineStyle.Single;
            shape2.LineFormat.Weight = 3;
            shape2.LineFormat.ForeColor = Color.Red;
            shape2.LineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            shape2.Text = "DashDotDot Line";

            // Salva la cartella di lavoro
            workbook.Save("LineDashStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


