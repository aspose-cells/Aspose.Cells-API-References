---
title: "Cells.MaxDataColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Maximaler Spaltenindex einer Zelle, die Daten enthält"
type: docs
url: /de/net/aspose.cells/cells/maxdatacolumn/
---
## Cells.MaxDataColumn property

Maximaler Spaltenindex der Zelle, die Daten enthält.

```csharp
public int MaxDataColumn { get; }
```

### Hinweise

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Erhalte den maximalen Daten-Spaltenindex (nullbasiert)
            int maxColumn = worksheet.Cells.MaxDataColumn;
            Console.WriteLine("Max Data Column: " + maxColumn);

            // Exportiere Daten mit MaxDataColumn
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 
                worksheet.Cells.MaxDataRow + 1, 
                worksheet.Cells.MaxDataColumn + 1);

            // Exportierte Daten anzeigen
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

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


