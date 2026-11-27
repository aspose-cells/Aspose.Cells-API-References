---
title: "Worksheet.RemoveAutoFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Tar bort autofiltret i arbetsbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/removeautofilter/
---
## Worksheet.RemoveAutoFilter method

Tar bort autofiltret i kalkylbladet.

```csharp
public void RemoveAutoFilter()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAutoFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:A3";
            
            Console.WriteLine("AutoFilter applied: " + worksheet.HasAutofilter);
            
            // Ta bort autofilter
            worksheet.RemoveAutoFilter();
            
            Console.WriteLine("AutoFilter after removal: " + worksheet.HasAutofilter);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


