---
title: "FindOptions.ValueTypeSensitive"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions-egenskapen. Anger om den sökta cellvärdestypen ska vara densamma som den sökta nyckeln"
type: docs
url: /sv/net/aspose.cells/findoptions/valuetypesensitive/
---
## FindOptions.ValueTypeSensitive property

Anger om den sökta cellvärdestypen ska vara densamma som den sökta nyckeln.

```csharp
public bool ValueTypeSensitive { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyValueTypeSensitiveDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till olika värdetyper i celler
            worksheet.Cells["A1"].PutValue("100"); // Stored as string
            worksheet.Cells["A2"].PutValue(100);   // Stored as number
            worksheet.Cells["A3"].PutValue("100.0"); // Stored as string
            worksheet.Cells["A4"].PutValue(100.0);   // Stored as number

            // Skapa sökalternativ med ValueTypeSensitive = true
            FindOptions options = new FindOptions();
            options.ValueTypeSensitive = true;
            options.LookAtType = LookAtType.EntireContent;

            // Sök efter talet 100 (hittar inte strängen "100")
            Cell foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found cell with number 100: " + (foundCell != null ? foundCell.Name : "Not found"));

            // Sök efter strängen "100" (hittar inte talet 100)
            foundCell = worksheet.Cells.Find("100", null, options);
            Console.WriteLine("Found cell with string \"100\": " + (foundCell != null ? foundCell.Name : "Not found"));

            // Ändra till ValueTypeSensitive = false
            options.ValueTypeSensitive = false;
            
            // Nu kommer båda sökningarna att hitta vilken cell som helst med "100" eller 100
            foundCell = worksheet.Cells.Find(100, null, options);
            Console.WriteLine("Found any 100 (type insensitive): " + (foundCell != null ? foundCell.Name : "Not found"));
        }
    }
}
```

### Se även

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


