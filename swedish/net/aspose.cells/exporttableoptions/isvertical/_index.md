---
title: "ExportTableOptions.IsVertical"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions-egenskap. Sant om en rad i Workbook-filen representerar en rad i DataTable. Falskt om en kolumn i Workbook-filen representerar en rad i DataTable"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/isvertical/
---
## ExportTableOptions.IsVertical property

True om en rad i Workbook-filen representerar en rad i DataTable. False om en kolumn i Workbook-filen representerar en rad i DataTable.

```csharp
public bool IsVertical { get; set; }
```

### Exempel

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
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa exempeldata i kalkylbladet
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(25);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(30);

            // Skapa DataTable
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));

            // Ställ in ExportTableOptions med IsVertical = true
            ExportTableOptions options = new ExportTableOptions();
            options.IsVertical = true;
            options.ExportColumnName = true;
            options.DataTable = dt;

            // Exportera data vertikalt
            cells.ExportDataTable(0, 0, 2, 2, options);

            // Visa den exporterade DataTable
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}");
            }
        }
    }
}
```

### Se även

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


