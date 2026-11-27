---
title: "ImportTableOptions.TotalRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions-egenskap. Hämtar eller anger totalt antal rader att importera från datakällan. 1 betyder alla rader i den angivna datakällan"
type: docs
url: /sv/net/aspose.cells/importtableoptions/totalrows/
---
## ImportTableOptions.TotalRows property

Hämtar eller anger totalt antal rader att importera från datakällan. -1 betyder alla rader i den angivna datakällan.

```csharp
public int TotalRows { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalRowsDemo
    {
        public static void Run()
        {
            // Skapa en exempel-DataTable
            DataTable table = new DataTable("TestTable");
            table.Columns.Add("Column1", typeof(string));
            table.Columns.Add("Column2", typeof(int));
            
            // Lägg till exempeldata
            table.Rows.Add("Item1", 100);
            table.Rows.Add("Item2", 200);
            table.Rows.Add("Item3", 300);

            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ImportTableOptions med TotalRows satt till 2 (kommer bara att importera de två första raderna)
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalRows = 2 // Only import 2 rows from the DataTable
            };

            // Importera data med de angivna alternativen
            worksheet.Cells.ImportData(table, 0, 0, options);

            // Spara arbetsboken
            workbook.Save("ImportWithTotalRows.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Data imported with TotalRows=2. Only first 2 rows were imported.");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


