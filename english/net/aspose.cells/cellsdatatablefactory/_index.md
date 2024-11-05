---
title: Class CellsDataTableFactory
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CellsDataTableFactory class. Utility to build ICellsDataTable from custom objects for users convenience
type: docs
url: /net/aspose.cells/cellsdatatablefactory/
---
## CellsDataTableFactory class

Utility to build ICellsDataTable from custom objects for user's convenience.

```csharp
public class CellsDataTableFactory
```

## Methods

| Name | Description |
| --- | --- |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance)(double[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_6)(ICollection) | Creates ICellsDataTable from given collection. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_3)(int[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_7)(object[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_1)(double[], bool) | Creates ICellsDataTable from given sequence of double values. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_2)(double[], string[]) | Creates ICellsDataTable from given sequence of double values. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_4)(int[], bool) | Creates ICellsDataTable from given sequence of int values. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_5)(int[], string[]) | Creates ICellsDataTable from given sequence of int values. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_8)(object[], bool) | Creates ICellsDataTable from given sequence of objects. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_9)(object[], string[]) | Creates ICellsDataTable from given sequence of objects. |

### Examples

```csharp
[C#]

using Aspose.Cells;
using System;
using System.Collections.Generic;

namespace Demos
{
    public class CellsDataTableFactoryDemo
    {
        public static void RunDemo()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Get the CellsDataTableFactory instance from the workbook
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Create an ICellsDataTable instance from the custom data list
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Import the data table into the worksheet starting at cell A1
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Save the workbook
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
            workbook.Save("CellsDataTableFactoryDemo.pdf");
        }
    }

    // Custom data class
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


