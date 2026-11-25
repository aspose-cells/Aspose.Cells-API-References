---
title: "ExportTableOptions.IsVertical"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ExportTableOptions proprietà. True se una riga nel file Workbook rappresenta una riga nel DataTable. False se una colonna nel file Workbook rappresenta una riga nel DataTable"
type: docs
url: /it/net/aspose.cells/exporttableoptions/isvertical/
---
## ExportTableOptions.IsVertical property

True se una riga nel file Workbook rappresenta una riga nella DataTable. False se una colonna nel file Workbook rappresenta una riga nella DataTable.

```csharp
public bool IsVertical { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyIsVerticalDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea dati di esempio nel foglio di lavoro
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(25);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(30);

            // Crea DataTable
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));

            // Imposta ExportTableOptions con IsVertical = true
            ExportTableOptions options = new ExportTableOptions();
            options.IsVertical = true;
            options.ExportColumnName = true;
            options.DataTable = dt;

            // Esporta i dati verticalmente
            cells.ExportDataTable(0, 0, 2, 2, options);

            // Visualizza la DataTable esportata
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}");
            }
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


