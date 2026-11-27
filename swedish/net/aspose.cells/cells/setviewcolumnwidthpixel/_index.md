---
title: "Cells.SetViewColumnWidthPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Ställer in kolumnens bredd i olika vyer"
type: docs
url: /sv/net/aspose.cells/cells/setviewcolumnwidthpixel/
---
## Cells.SetViewColumnWidthPixel method

Ställer in kolumnens bredd i olika vyer.

```csharp
public void SetViewColumnWidthPixel(int column, int pixels)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindexet. |
| pixlar | Int32 | Bredden i enhet pixlar. |

### Anmärkningar

Om den aktuella vystyptypen är PageLayoutView, är kolumnens bredd densamma som den utskrivna bredden.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetViewColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Ange exempeldata
            sheet.Cells[0, 0].Value = "Sample Text";

            // Beräkna pixelbredd (100 pixlar i detta exempel)
            int pixelWidth = 100;

            // Ställ in kolumnbredd i pixlar
            sheet.Cells.SetViewColumnWidthPixel(0, pixelWidth);

            // Spara arbetsboken
            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


