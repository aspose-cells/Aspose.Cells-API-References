---
title: "FilterColumnCollection.GetByIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FilterColumnCollection. Restituisce un singolo oggetto Filter da una collezione"
type: docs
url: /it/net/aspose.cells/filtercolumncollection/getbyindex/
---
## FilterColumnCollection.GetByIndex method

Restituisce un singolo oggetto Filter da una raccolta.

```csharp
public FilterColumn GetByIndex(int index)
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnCollectionMethodGetByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(30);

            worksheet.AutoFilter.Range = "A1:B3";
            FilterColumnCollection filterColumns = worksheet.AutoFilter.FilterColumns;

            worksheet.AutoFilter.AddFilter(1, "25");
            worksheet.AutoFilter.Refresh();

            FilterColumn filterColumn = filterColumns.GetByIndex(0);
            Console.WriteLine("Filter column index: " + filterColumn.FieldIndex);

            workbook.Save("FilterColumnCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


