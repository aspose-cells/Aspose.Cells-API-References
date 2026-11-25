---
title: "FilterColumnCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FilterColumnCollection."
type: docs
url: /it/net/aspose.cells/filtercolumncollection/removeat/
---
## FilterColumnCollection.RemoveAt method

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 |  |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnCollectionMethodRemoveAtWithInt32Demo
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

            Console.WriteLine("Filters before removal: " + filterColumns.Count);
            filterColumns.RemoveAt(0);
            Console.WriteLine("Filters after removal: " + filterColumns.Count);

            workbook.Save("FilterColumnCollectionRemoveAtDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


