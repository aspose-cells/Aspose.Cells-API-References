---
title: "Cells.MaxDataColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Indice massimo della colonna della cella che contiene dati"
type: docs
url: /it/net/aspose.cells/cells/maxdatacolumn/
---
## Cells.MaxDataColumn property

Indice di colonna massimo della cella che contiene dati.

```csharp
public int MaxDataColumn { get; }
```

### Osservazioni

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Ottieni l'indice massimo della colonna dati (basato su zero)
            int maxColumn = worksheet.Cells.MaxDataColumn;
            Console.WriteLine("Max Data Column: " + maxColumn);

            // Esporta i dati usando MaxDataColumn
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 
                worksheet.Cells.MaxDataRow + 1, 
                worksheet.Cells.MaxDataColumn + 1);

            // Visualizza i dati esportati
            Console.WriteLine("Exported Data:");
            foreach (DataRow row in dataTable.Rows)
            {
                for (int i = 0; i <= maxColumn; i++)
                {
                    Console.Write(row[i] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


