---
title: "Worksheet.IsOutlineShown"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑egenskap. Anger om konturen ska visas"
type: docs
url: /sv/net/aspose.cells/worksheet/isoutlineshown/
---
## Worksheet.IsOutlineShown property

Anger om konturen ska visas.

```csharp
public bool IsOutlineShown { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsOutlineShownDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in att konturen ska visas
            worksheet.IsOutlineShown = true;
            Console.WriteLine("Outline shown: " + worksheet.IsOutlineShown);
            
            // Spara och ladda om för att demonstrera beständighet
            string filePath = "IsOutlineShownDemo.xlsx";
            workbook.Save(filePath);
            
            Workbook loadedWorkbook = new Workbook(filePath);
            Console.WriteLine("Reloaded - Outline shown: " + loadedWorkbook.Worksheets[0].IsOutlineShown);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


