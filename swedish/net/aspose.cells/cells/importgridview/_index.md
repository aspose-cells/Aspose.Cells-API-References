---
title: "Cells.ImportGridView"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Importerar en grid view till dessa celler"
type: docs
url: /sv/net/aspose.cells/cells/importgridview/
---
## Cells.ImportGridView method

Importerar en rutnätsvy till dessa celler.

```csharp
public int ImportGridView(GridView gridView, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| gridView | GridView | Det grid view-objektet. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| alternativ | ImportTableOptions | importalternativ. |

### Returvärde

Radnumret.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en DataTable för att simulera GridView-data
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Price");
            dataTable.Columns.Add("Stock");

            dataTable.Rows.Add("Product A", 100.5, 50);
            dataTable.Rows.Add("Product B", 200.75, 30);
            dataTable.Rows.Add("Product C", 150.25, 75);

            try
            {
                // Skapa ImportTableOptions
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;
                options.InsertRows = true;

                // Importera DataTable-data som börjar på cell B3 (rad 2, kolumn 1)
                worksheet.Cells.ImportData(dataTable, 2, 1, options);

                Console.WriteLine("Data imported successfully starting at cell B3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


