---
title: "ListObject.Comment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject egenskap. Hämtar och sätter kommentaren för tabellen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/comment/
---
## ListObject.Comment property

Hämtar och anger kommentaren för tabellen.

```csharp
public string Comment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyCommentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för listobjektet
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(100);

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];

            // Ställ in och demonstrera Comment-egenskapen
            listObj.Comment = "This is a sample comment for the list object";
            Console.WriteLine("List Object Comment: " + listObj.Comment);

            // Ändra storlek på listobjektet för att inkludera mer data
            listObj.Resize(0, 0, 2, 1, true);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(200);

            // Spara arbetsboken
            workbook.Save("ListObjectCommentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


