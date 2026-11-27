---
title: "ListObject.ShowTableStyleFirstColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject-egenskap. Anger om den första kolumnen i tabellen är den stil som tillämpas på"
type: docs
url: /sv/net/aspose.cells.tables/listobject/showtablestylefirstcolumn/
---
## ListObject.ShowTableStyleFirstColumn property

Anger om den första kolumnen i tabellen är den stil som tillämpas på.

```csharp
public bool ShowTableStyleFirstColumn { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleFirstColumnDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["B4"].PutValue(3.2);

            // Skapa ett listobjekt
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];
            
            // Applicera stil på första kolumnen
            listObject.ShowTableStyleFirstColumn = true;
            
            // Spara arbetsboken
            workbook.Save("ListObjectShowFirstColumnStyle.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("File saved with first column style applied to the table.");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


