---
title: "ListObject.AlternativeText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject egenskap. Hämtar och sätter den alternativa texten"
type: docs
url: /sv/net/aspose.cells.tables/listobject/alternativetext/
---
## ListObject.AlternativeText property

Hämtar och anger den alternativa texten.

```csharp
public string AlternativeText { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa ett listobjekt/tabell
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Ange alternativ text och beskrivning
            table.AlternativeText = "Test";
            table.AlternativeDescription = "aSXADCS";
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Läs om och verifiera
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedTable = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedTable.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedTable.AlternativeDescription);
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


