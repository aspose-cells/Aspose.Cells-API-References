---
title: "AutoFilter.ShowAll"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Visa alla rader"
type: docs
url: /sv/net/aspose.cells/autofilter/showall/
---
## AutoFilter.ShowAll method

Visa alla rader.

```csharp
public void ShowAll()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodShowAllDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Filtrera för att endast visa "Apple"
            worksheet.AutoFilter.Filter(0, "Apple");
            
            // Visa all data igen
            worksheet.AutoFilter.ShowAll();
            
            // Spara arbetsboken
            workbook.Save("ShowAllDemoOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


