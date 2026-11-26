---
title: "FilterColumnCollection.GetByIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FilterColumnCollection. Devuelve un único objeto Filter de una colección"
type: docs
url: /es/net/aspose.cells/filtercolumncollection/getbyindex/
---
## FilterColumnCollection.GetByIndex method

Devuelve un único objeto Filter de una colección.

```csharp
public FilterColumn GetByIndex(int index)
```

### Ejemplos

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

### Ver también

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


