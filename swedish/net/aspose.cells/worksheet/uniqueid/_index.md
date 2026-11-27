---
title: "Worksheet.UniqueId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar och anger det unika id:t, det är samma som 15DB5C3CA5A148AF8F253D86AC232D4F"
type: docs
url: /sv/net/aspose.cells/worksheet/uniqueid/
---
## Worksheet.UniqueId property

Hämtar och anger det unika id:t, det är samma som {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

```csharp
public string UniqueId { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyUniqueIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Generera ett unikt ID för kalkylbladet
            string uniqueId = "{" + Guid.NewGuid().ToString() + "}";
            
            // Ange UniqueId-egenskapen för det första kalkylbladet
            workbook.Worksheets[0].UniqueId = uniqueId;
            
            // Spara arbetsboken
            string outputPath = "SheetUniqueIdDemo.xlsx";
            workbook.Save(outputPath);
            
            // Läs in arbetsboken igen för att verifiera att UniqueId kvarstår
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Skriv ut UniqueId för att demonstrera funktionaliteten
            Console.WriteLine("Worksheet UniqueId: " + loadedWorkbook.Worksheets[0].UniqueId);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


