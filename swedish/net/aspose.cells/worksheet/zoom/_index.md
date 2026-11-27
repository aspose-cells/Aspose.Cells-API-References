---
title: "Worksheet.Zoom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑egenskap. Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400"
type: docs
url: /sv/net/aspose.cells/worksheet/zoom/
---
## Worksheet.Zoom property

Representerar skalningsfaktorn i procent. Den bör vara mellan 10 och 400.

```csharp
public int Zoom { get; set; }
```

### Anmärkningar

Vänligen ange vytypen först.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyZoomDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in zoomfaktorn till 120%
            worksheet.Zoom = 120;
            
            // Visa den aktuella zoomfaktorn
            Console.WriteLine("Current worksheet zoom: " + worksheet.Zoom + "%");
            
            // Spara arbetsboken
            workbook.Save("WorksheetZoomDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


