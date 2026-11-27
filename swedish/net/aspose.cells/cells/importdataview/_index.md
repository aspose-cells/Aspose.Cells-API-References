---
title: "Cells.ImportDataView"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Importerar en DataView till ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/cells/importdataview/
---
## Cells.ImportDataView method

Importerar en DataView till ett kalkylblad.

```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataView | DataView | DataView-objektet som ska importeras. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |

### Returvärde

Totalt antal importerade rader

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataViewWithDataViewInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa exempel på DataTable
            DataTable table = new DataTable("Products");
            table.Columns.Add("ID", typeof(int));
            table.Columns.Add("Name", typeof(string));
            table.Columns.Add("Price", typeof(decimal));

            // Lägg till exempeldata
            table.Rows.Add(1, "Laptop", 999.99m);
            table.Rows.Add(2, "Smartphone", 699.99m);
            table.Rows.Add(3, "Tablet", 399.99m);

            // Skapa DataView från DataTable
            DataView dataView = new DataView(table);

            // Importera DataView till kalkylbladet med start på rad 0, kolumn 0
            cells.ImportDataView(dataView, 0, 0);

            // Spara arbetsboken
            workbook.Save("ImportDataViewOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


