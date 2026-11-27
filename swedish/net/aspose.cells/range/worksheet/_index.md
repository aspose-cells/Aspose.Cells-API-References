---
title: "Range.Worksheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Hämtar Worksheet-objektet som innehåller detta range"
type: docs
url: /sv/net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

Hämtar `Worksheet`-objektet som innehåller detta range.

```csharp
public Worksheet Worksheet { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett namngivet område
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            // Definiera ett namngivet range
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Hämta range efter namn (specificera `Range` fullt för att undvika tvetydighet)
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("MyRange");
            
            // Demonstrera användning av Worksheet-egenskap
            Console.WriteLine("Range belongs to worksheet: " + range.Worksheet.Name);
            
            // Använd Worksheet-egenskap för att modifiera celler
            range.Worksheet.Cells["A1"].PutValue("Updated");
            
            // Spara arbetsboken
            workbook.Save("RangePropertyWorksheetDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


