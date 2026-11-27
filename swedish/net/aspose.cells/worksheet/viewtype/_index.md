---
title: "Worksheet.ViewType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar och anger vytypen"
type: docs
url: /sv/net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

Hämtar och anger vytypen.

```csharp
public ViewType ViewType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyViewTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in vytypen till PageLayoutView och aktivera linjal
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsRulerVisible = true;
            
            // Lägg till lite exempelinnehåll för att demonstrera vyn
            worksheet.Cells["A1"].PutValue("Page Layout View Demo");
            worksheet.Cells["A2"].PutValue("Ruler is visible in this view");
            
            // Spara arbetsboken
            workbook.Save("WorksheetViewTypeDemo.xlsx");
            
            Console.WriteLine("Worksheet ViewType demo completed successfully.");
        }
    }
}
```

### Se även

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


