---
title: "ListColumn.TotalsCalculation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumn egenskap. Hämtar och anger typen av beräkning i totalsraden för listkolumnen"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/totalscalculation/
---
## ListColumn.TotalsCalculation property

Hämtar och anger typen av beräkning i totalsraden för listkolumnen.

```csharp
public TotalsCalculation TotalsCalculation { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyTotalsCalculationDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("Item 3");
            worksheet.Cells["B4"].PutValue(200);

            // Skapa ett listobjekt
            int listObjIndex = worksheet.ListObjects.Add(0, 0, 4, 1, true);
            ListObject listObj = worksheet.ListObjects[listObjIndex];
            listObj.ShowTotals = true;
            
            // Ange totalsberäkning för den andra kolumnen
            listObj.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Spara arbetsboken
            workbook.Save("ListColumnTotalsCalculationDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TotalsCalculation](../../totalscalculation/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


