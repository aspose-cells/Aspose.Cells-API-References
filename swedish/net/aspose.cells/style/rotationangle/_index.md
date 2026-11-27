---
title: "Style.RotationAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Representerar textrotationsvinkel"
type: docs
url: /sv/net/aspose.cells/style/rotationangle/
---
## Style.RotationAngle property

Representerar textrotationsvinkeln.

```csharp
public int RotationAngle { get; set; }
```

### Anmärkningar

0: Inte roterad.

255: Uppifrån och ner.

-90: Downward.

90: Uppåt.

Du kan ange 255 eller ett värde mellan -90 och 90.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil med olika rotationsvinklar
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

            // Spara arbetsboken
            workbook.Save("output_rotation_angles.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


