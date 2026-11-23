---
title: "DataSorterKey.Order"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorterKey. Indique l'ordre du tri"
type: docs
url: /fr/net/aspose.cells/datasorterkey/order/
---
## DataSorterKey.Order property

Indique l'ordre du tri.

```csharp
public SortOrder Order { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(80);

            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Sort by Score column

            CellArea area = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            sorter.Sort(worksheet.Cells, area);

            // Démontrer l'utilisation de la propriété Order
            DataSorterKey key = sorter.Keys[0];
            Console.WriteLine("Key Order: " + key.Order);

            workbook.Save("DataSorterKeyOrderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SortOrder](../../sortorder/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


