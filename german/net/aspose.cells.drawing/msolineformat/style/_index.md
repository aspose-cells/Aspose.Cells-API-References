---
title: "MsoLineFormat.Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormat-Eigenschaft. Gibt ein Style-Objekt zurück, das den Stil des angegebenen Bereichs darstellt"
type: docs
url: /de/net/aspose.cells.drawing/msolineformat/style/
---
## MsoLineFormat.Style property

Gibt ein Style-Objekt zurück, das den Stil des angegebenen Bereichs darstellt.

```csharp
public MsoLineStyle Style { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Linienform hinzufügen
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);

            // Hole das Linienformat
            MsoLineFormat lineFormat = line.LineFormat;

            // Lege Zeilenstil-Eigenschaften fest
            lineFormat.Style = MsoLineStyle.ThickBetweenThin;
            lineFormat.ForeColor = System.Drawing.Color.Red;
            lineFormat.BackColor = System.Drawing.Color.White;
            lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 3.0;

            // Erstelle eine weitere Linie zum Vergleich
            Aspose.Cells.Drawing.LineShape line2 = worksheet.Shapes.AddLine(5, 25, 100, 150, 10, 10);
            MsoLineFormat lineFormat2 = line2.LineFormat;

            // Kopiere den Stil von der ersten Linie zur zweiten Linie
            lineFormat2.Style = lineFormat.Style;
            lineFormat2.ForeColor = lineFormat.ForeColor;
            lineFormat2.BackColor = lineFormat.BackColor;
            lineFormat2.DashStyle = lineFormat.DashStyle;
            lineFormat2.Transparency = lineFormat.Transparency;
            lineFormat2.Weight = lineFormat.Weight;

            // Speichere die Arbeitsmappe
            workbook.Save("MsoLineFormatStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


