---
title: "FilterColumn.FieldIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumn-egenskapen. Hämtar och anger kolumnförskjutningen i intervallet"
type: docs
url: /sv/net/aspose.cells/filtercolumn/fieldindex/
---
## FilterColumn.FieldIndex property

Hämtar och anger kolumnförskjutningen i intervallet.

```csharp
public int FieldIndex { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Employees");
            worksheet.Cells["A2"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["A3"].PutValue("Marketing");
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["A4"].PutValue("IT");
            worksheet.Cells["B4"].PutValue(12);

            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:B4";
            
            // Lägg till filter i första kolumnen (Department)
            worksheet.AutoFilter.AddFilter(0, "Sales");

            // Hämta filterkolumnen
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            
            // Demonstrera FieldIndex-egenskapen
            Console.WriteLine("Filter is applied on column index: " + filterColumn.FieldIndex);
            
            // Uppdatera och spara
            worksheet.AutoFilter.Refresh();
            workbook.Save("FilterColumnFieldIndexDemo.xlsx");
        }
    }
}
```

### Se även

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


