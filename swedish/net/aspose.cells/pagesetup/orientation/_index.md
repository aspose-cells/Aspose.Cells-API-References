---
title: "PageSetup.Orientation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar sidans utskriftsorientering"
type: docs
url: /sv/net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

Representerar sidans utskriftsorientering.

```csharp
public PageOrientationType Orientation { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrientationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in sidorientering till Liggande
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            
            // Lägg till några exempeldata för att demonstrera effekten
            worksheet.Cells["A1"].PutValue("Landscape Orientation Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data Row {i}");
            }
            
            // Spara arbetsboken
            workbook.Save("PageOrientationDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


