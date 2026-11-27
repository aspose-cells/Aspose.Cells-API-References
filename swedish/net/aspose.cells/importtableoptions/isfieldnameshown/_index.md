---
title: "ImportTableOptions.IsFieldNameShown"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions-egenskap. Anger om fältnamnet ska importeras"
type: docs
url: /sv/net/aspose.cells/importtableoptions/isfieldnameshown/
---
## ImportTableOptions.IsFieldNameShown property

Anger om fältnamnet ska importeras.

```csharp
public bool IsFieldNameShown { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFieldNameShownDemo
    {
        public static void Run()
        {
            // Skapa en exempel-DataTable
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Product");
            
            // Lägg till exempeldata
            table.Rows.Add(1, "Laptop");
            table.Rows.Add(2, "Smartphone");
            table.Rows.Add(3, "Tablet");

            // Skapa en arbetsbok och importera data med fältnamn visade
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;  // Show field names
            options.InsertRows = true;       // Insert new rows
            
            // Importera data med start från rad 5, kolumn 0
            cells.ImportData(table, 5, 0, options);
            
            // Spara arbetsboken
            workbook.Save("ImportDataWithFieldNames.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


