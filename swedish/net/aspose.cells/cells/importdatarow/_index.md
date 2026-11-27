---
title: "Cells.ImportDataRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Importerar en DataRow till Excel-filen"
type: docs
url: /sv/net/aspose.cells/cells/importdatarow/
---
## Cells.ImportDataRow method

Importerar en DataRow till Excel-filen.

```csharp
public void ImportDataRow(DataRow dataRow, int row, int firstColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataRow | DataRow | DataRow-objekt. |
| row | Int32 | Radindex. |
| firstColumn | Int32 | Första kolumnens index. |

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataRowWithDataRowInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa en exempel-DataTable
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Lägg till exempeldata
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Importera den första raden från DataTable till kalkylbladet med start i rad 0, kolumn 0
            cells.ImportDataRow(dataTable.Rows[0], 0, 0);

            // Spara arbetsboken
            workbook.Save("ImportDataRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


