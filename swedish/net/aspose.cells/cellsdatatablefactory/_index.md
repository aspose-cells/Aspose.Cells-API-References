---
title: "Klass CellsDataTableFactory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellsDataTableFactory-klass. Verktyg för att bygga ICellsDataTable från anpassade objekt för användarnas bekvämlighet"
type: docs
url: /sv/net/aspose.cells/cellsdatatablefactory/
---
## CellsDataTableFactory class

Verktyg för att bygga ICellsDataTable från anpassade objekt för användarens bekvämlighet.

```csharp
public class CellsDataTableFactory
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance)(double[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_6)(ICollection) | Skapar ICellsDataTable från given samling. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_3)(int[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_8)(object[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_1)(double[], bool) | Skapar ICellsDataTable från given sekvens av double‑värden. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_2)(double[], string[]) | Skapar ICellsDataTable från given sekvens av double‑värden. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_7)(ICollection, bool) | Skapar ICellsDataTable från given samling. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_4)(int[], bool) | Skapar ICellsDataTable från given sekvens av heltalsvärden. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_5)(int[], string[]) | Skapar ICellsDataTable från given sekvens av heltalsvärden. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_9)(object[], bool) | Skapar ICellsDataTable från given sekvens av objekt. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_10)(object[], string[]) | Skapar ICellsDataTable från given sekvens av objekt. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_11)(object[][], bool, string[]) | Skapar en ICellsDataTable från en given sekvens av objekt. |

### Exempel

```csharp
using Aspose.Cells;
using System;
using System.Collections.Generic;

namespace AsposeCellsExamples
{
    public class CellsDataTableFactoryDemo
    {
        public static void RunDemo()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Hämta CellsDataTableFactory‑instansen från arbetsboken
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Skapa en ICellsDataTable‑instans från den anpassade datalistan
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Importera datatabellen till kalkylbladet med start i cell A1
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Spara arbetsboken
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
            workbook.Save("CellsDataTableFactoryDemo.pdf");
        }
    }

    // Anpassad dataklass
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


