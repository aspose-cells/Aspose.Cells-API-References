---
title: "PageSetup.Zoom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400"
type: docs
url: /sv/net/aspose.cells/pagesetup/zoom/
---
## PageSetup.Zoom property

Anger skalningsfaktorn i procent. Den bör vara mellan 10 och 400.

```csharp
public int Zoom { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyZoomDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in zoomnivå till 150%
            worksheet.PageSetup.Zoom = 150;
            
            // Skriv ut aktuell zoomnivå
            Console.WriteLine("Current Zoom Level: " + worksheet.PageSetup.Zoom);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


