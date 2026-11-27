---
title: "ListObject.ShowTableStyleRowStripes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject egenskap. Indikerar om radrandig formatering tillämpas på"
type: docs
url: /sv/net/aspose.cells.tables/listobject/showtablestylerowstripes/
---
## ListObject.ShowTableStyleRowStripes property

Anger om radrandig formatering är tillämpad på.

```csharp
public bool ShowTableStyleRowStripes { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleRowStripesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);

            // Skapa ett listobjekt
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];

            // Demonstrera egenskapen ShowTableStyleRowStripes
            Console.WriteLine("Before: ShowTableStyleRowStripes = " + listObject.ShowTableStyleRowStripes);
            listObject.ShowTableStyleRowStripes = false;
            Console.WriteLine("After: ShowTableStyleRowStripes = " + listObject.ShowTableStyleRowStripes);

            // Spara arbetsboken
            workbook.Save("ListObjectShowTableStyleRowStripesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


