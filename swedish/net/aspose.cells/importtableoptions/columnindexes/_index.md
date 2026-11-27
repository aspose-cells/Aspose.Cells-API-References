---
title: "ImportTableOptions.ColumnIndexes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions egenskap. Hämtar eller anger kolumner0baserade att importera från datakällan. null betyder att alla kolumner ska importeras"
type: docs
url: /sv/net/aspose.cells/importtableoptions/columnindexes/
---
## ImportTableOptions.ColumnIndexes property

Hämtar eller anger kolumnerna (0‑baserade) som ska importeras från datakällan. null betyder att alla kolumner ska importeras.

```csharp
public int[] ColumnIndexes { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyColumnIndexesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempel på DataTable
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Lägg till exempeldata
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);
            dataTable.Rows.Add(3, "Product C", 39.99m);

            // Ställ in importalternativ för att endast importera kolumner på index 0 och 2 (ID och Pris)
            ImportTableOptions options = new ImportTableOptions();
            options.ColumnIndexes = new int[] { 0, 2 };
            options.IsFieldNameShown = true;

            // Importera data med angivna kolumnindex
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Spara arbetsboken
            workbook.Save("ColumnIndexesDemo.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


