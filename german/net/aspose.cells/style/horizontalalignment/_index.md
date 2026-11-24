---
title: "Style.HorizontalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style property. Gibt den horizontalen Ausrichtungstyp des Textes in einer Zelle zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells/style/horizontalalignment/
---
## Style.HorizontalAlignment property

Liest oder setzt den horizontalen Ausrichtungstyp des Textes in einer Zelle.

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Text in Zellen festlegen
            cells["A1"].PutValue("Left Aligned");
            cells["A2"].PutValue("Center Aligned");
            cells["A3"].PutValue("Right Aligned");

            // Stilobjekte abrufen
            Style styleLeft = cells["A1"].GetStyle();
            Style styleCenter = cells["A2"].GetStyle();
            Style styleRight = cells["A3"].GetStyle();

            // Horizontale Ausrichtung festlegen
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            styleRight.HorizontalAlignment = TextAlignmentType.Right;

            // Stile auf Zellen anwenden
            cells["A1"].SetStyle(styleLeft);
            cells["A2"].SetStyle(styleCenter);
            cells["A3"].SetStyle(styleRight);

            // Speichere die Arbeitsmappe
            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


