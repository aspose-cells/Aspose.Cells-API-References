---
title: "StyleFlag.VerticalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Vertikale Ausrichtungseinstellung wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/verticalalignment/
---
## StyleFlag.VerticalAlignment property

Die Einstellung für die vertikale Ausrichtung wird angewendet.

```csharp
public bool VerticalAlignment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Erstellen Sie einen Stil mit vertikaler Ausrichtung
            Style style = workbook.CreateStyle();
            style.VerticalAlignment = TextAlignmentType.Center;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.Font.Color = Color.Blue;

            // Erstellen Sie ein Style-Flag, um nur vertikale Ausrichtung und Schriftfarbe anzuwenden
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.VerticalAlignment = true;
            styleFlag.FontColor = true;

            // Wenden Sie den Stil auf die erste Zeile mit dem Style-Flag an
            Row row = sheet.Cells.Rows[0];
            row.ApplyStyle(style, styleFlag);

            // Setzen Sie etwas Text in die Zellen, um den Effekt zu sehen
            sheet.Cells["A1"].PutValue("Vertically Centered");
            sheet.Cells["B1"].PutValue("Blue Text");

            // Speichere die Arbeitsmappe
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


