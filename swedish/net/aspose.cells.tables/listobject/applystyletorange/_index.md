---
title: "ListObject.ApplyStyleToRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject metod. Applicera tabellstilen på området"
type: docs
url: /sv/net/aspose.cells.tables/listobject/applystyletorange/
---
## ListObject.ApplyStyleToRange method

Tillämpa tabellstilen på intervallet.

```csharp
public void ApplyStyleToRange()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodApplyStyleToRangeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att skapa ett listobjekt
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = worksheet.ListObjects[index];

            // Applicera stil på området för listobjektet
            listObject.ApplyStyleToRange();

            // Verifiera att stilen har tillämpats genom att kontrollera en cells förgrundsfärg
            Style style = worksheet.Cells["A1"].GetStyle();
            Console.WriteLine("Foreground color applied: " + style.ForegroundColor);

            // Konvertera listobjekt till område och verifiera
            listObject.ConvertToRange();
            Console.WriteLine("List objects count after conversion: " + worksheet.ListObjects.Count);
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


