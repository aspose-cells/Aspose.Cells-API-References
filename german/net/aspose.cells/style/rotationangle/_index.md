---
title: "Style.RotationAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt den Textdrehwinkel an."
type: docs
url: /de/net/aspose.cells/style/rotationangle/
---
## Style.RotationAngle property

Stellt den Textdrehwinkel dar.

```csharp
public int RotationAngle { get; set; }
```

### Hinweise

0: Nicht gedreht.

255: Von oben nach unten.

-90: Downward.

90: Aufwärts.

Sie können 255 oder einen Wert im Bereich von -90 bis 90 festlegen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Stil mit verschiedenen Drehwinkeln
            Style style1 = workbook.CreateStyle();
            style1.RotationAngle = -90;
            worksheet.Cells["B2"].PutValue("Text rotated -90°");
            worksheet.Cells["B2"].SetStyle(style1);

            Style style2 = workbook.CreateStyle();
            style2.RotationAngle = 90;
            worksheet.Cells["C3"].PutValue("Text rotated 90°");
            worksheet.Cells["C3"].SetStyle(style2);

            Style style3 = workbook.CreateStyle();
            style3.RotationAngle = 255;
            worksheet.Cells["D4"].PutValue("Text rotated 255°");
            worksheet.Cells["D4"].SetStyle(style3);

            // Speichere die Arbeitsmappe
            workbook.Save("output_rotation_angles.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


