---
title: "Cells.ImportGridView"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Importa una visualizzazione a griglia in queste celle"
type: docs
url: /it/net/aspose.cells/cells/importgridview/
---
## Cells.ImportGridView method

Importa una visualizzazione a griglia in queste celle.

```csharp
public int ImportGridView(GridView gridView, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| gridView | GridView | L'oggetto grid view. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| opzioni | ImportTableOptions | opzioni di importazione. |

### Valore di ritorno

Il numero della riga.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un DataTable per simulare i dati di GridView
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Price");
            dataTable.Columns.Add("Stock");

            dataTable.Rows.Add("Product A", 100.5, 50);
            dataTable.Rows.Add("Product B", 200.75, 30);
            dataTable.Rows.Add("Product C", 150.25, 75);

            try
            {
                // Crea ImportTableOptions
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;
                options.InsertRows = true;

                // Importa i dati del DataTable a partire dalla cella B3 (riga 2, colonna 1)
                worksheet.Cells.ImportData(dataTable, 2, 1, options);

                Console.WriteLine("Data imported successfully starting at cell B3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


