---
title: "ListObject.ShowTableStyleLastColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject egenskap. Anger om den sista kolumnen i tabellen är den stil som tillämpas på"
type: docs
url: /sv/net/aspose.cells.tables/listobject/showtablestylelastcolumn/
---
## ListObject.ShowTableStyleLastColumn property

Anger om den sista kolumnen i tabellen är den stil som tillämpas på.

```csharp
public bool ShowTableStyleLastColumn { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleLastColumnDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Skapa ett listobjekt
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];

            // Ställ in ShowTableStyleLastColumn-egenskapen
            listObject.ShowTableStyleLastColumn = true;

            // Spara arbetsboken
            workbook.Save("ListObjectShowLastColumnStyle.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("File saved with ShowTableStyleLastColumn enabled.");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


