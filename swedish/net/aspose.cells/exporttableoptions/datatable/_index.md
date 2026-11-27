---
title: "ExportTableOptions.DataTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions-egenskap. Hämtar och anger DataTable som kolumnernas datatyp är tilldelad"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/datatable/
---
## ExportTableOptions.DataTable property

Hämtar och anger DataTable där kolumnernas datatyp tilldelas.

```csharp
public DataTable DataTable { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyDataTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata i celler
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Text1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Text2");

            // Skapa DataTable och definiera kolumner
            DataTable dt = new DataTable();
            dt.Columns.Add("NumericData", typeof(double));
            dt.Columns.Add("TextData", typeof(string));

            // Konfigurera exportalternativ
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.Indexes = new int[] { 0, 1 }; // Export both columns
            options.DataTable = dt;

            // Exportera data till DataTable
            cells.ExportDataTable(0, 0, 3, 2, options);

            // Visa exporterad data
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["NumericData"]}, {row["TextData"]}");
            }
        }
    }
}
```

### Se även

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


