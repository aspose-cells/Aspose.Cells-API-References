---
title: "ListObject.AlternativeDescription"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject egenskap. Hämtar och anger den alternativa beskrivningen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/alternativedescription/
---
## ListObject.AlternativeDescription property

Hämtar och anger den alternativa beskrivningen.

```csharp
public string AlternativeDescription { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeDescriptionDemo
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

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Ange alternativ text och beskrivning
            listObject.AlternativeText = "Test";
            listObject.AlternativeDescription = "aSXADCS";

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Läs in igen och verifiera egenskaperna
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedListObject = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedListObject.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedListObject.AlternativeDescription);
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


