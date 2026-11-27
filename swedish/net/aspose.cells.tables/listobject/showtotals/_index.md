---
title: "ListObject.ShowTotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject‑egenskap. Hämtar och anger om denna tabell visar totalsrad"
type: docs
url: /sv/net/aspose.cells.tables/listobject/showtotals/
---
## ListObject.ShowTotals property

Hämtar och anger om den här TAble visar totalrad.

```csharp
public bool ShowTotals { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTotalsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa en tabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(8);

            // Skapa ett listobjekt/tabell
            int index = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject table = worksheet.ListObjects[index];

            // Aktivera totalsrad och ange en beräkning
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Spara arbetsboken
            workbook.Save("ListObjectShowTotalsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


