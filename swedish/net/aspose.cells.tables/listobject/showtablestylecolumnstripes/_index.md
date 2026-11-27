---
title: "ListObject.ShowTableStyleColumnStripes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject-egenskap. Anger om kolumnrandig formatering tillämpas på"
type: docs
url: /sv/net/aspose.cells.tables/listobject/showtablestylecolumnstripes/
---
## ListObject.ShowTableStyleColumnStripes property

Anger om kolumnrandig formatering är tillämpad på.

```csharp
public bool ShowTableStyleColumnStripes { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleColumnStripesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Skapa ett listobjekt och hämta referensen
            int listObjectIndex = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Ställ in egenskapen för kolumnrandor
            listObject.ShowTableStyleColumnStripes = true;
            
            // Spara arbetsboken
            workbook.Save("ListObjectWithColumnStripes.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with column stripes enabled.");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


