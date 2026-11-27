---
title: "ImportTableOptions.TotalColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions egenskap. Hämtar eller anger totalt antal kolumner att importera från datakällan. 1 betyder alla rader i den angivna datakällan"
type: docs
url: /sv/net/aspose.cells/importtableoptions/totalcolumns/
---
## ImportTableOptions.TotalColumns property

Hämtar eller anger totalt antal kolumner att importera från datakällan. -1 betyder att alla rader i den angivna datakällan importeras.

```csharp
public int TotalColumns { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalColumnsDemo
    {
        public static void Run()
        {
            // Skapa en exempel-DataTable
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Lägg till exempeldata
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in importalternativ med TotalColumns = 2 (kommer bara att importera de två första kolumnerna)
            ImportTableOptions importOptions = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalColumns = 2 // Only import first 2 columns (ID and Name)
            };

            // Importera data med start från cell A1
            cells.ImportData(dataTable, 0, 0, importOptions);

            // Spara arbetsboken
            workbook.Save("ImportWithTotalColumns.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Data imported with TotalColumns=2. Only first 2 columns were imported.");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


