---
title: "Worksheet.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Representerar om arbetsbladet är synligt"
type: docs
url: /sv/net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

Representerar om kalkylbladet är synligt.

```csharp
public bool IsVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till 3 arbetsblad
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Ställ in det andra arbetsbladet som dolt
            workbook.Worksheets[1].IsVisible = false;
            
            // Spara arbetsboken
            workbook.Save("WorksheetVisibilityDemo.xlsx");
            
            // Visa synlighetsstatus
            Console.WriteLine("Worksheet Visibility Status:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Console.WriteLine($"{workbook.Worksheets[i].Name}: {(workbook.Worksheets[i].IsVisible ? "Visible" : "Hidden")}");
            }
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


