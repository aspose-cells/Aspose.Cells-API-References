---
title: "Workbook.CellsDataTableFactory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar fabriken för att bygga ICellsDataTable från anpassade objekt"
type: docs
url: /sv/net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

Hämtar fabriken för att bygga ICellsDataTable från anpassade objekt

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### Exempel

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }

    public class WorkbookPropertyCellsDataTableFactoryDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Hämta CellsDataTableFactory från Workbook-egenskapen
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Skapa datatabell från lista
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Importera data till kalkylbladet
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Spara utdata
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


