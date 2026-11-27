---
title: "ImportTableOptions.InsertRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions egenskap. Anger om nya rader ska läggas till för import av dataposter"
type: docs
url: /sv/net/aspose.cells/importtableoptions/insertrows/
---
## ImportTableOptions.InsertRows property

Anger om nya rader ska läggas till för att importera dataregister.

```csharp
public bool InsertRows { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyInsertRowsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa exempeldatatabell
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            dataTable.Rows.Add(1, "Laptop", 999.99);
            dataTable.Rows.Add(2, "Monitor", 249.99);
            dataTable.Rows.Add(3, "Keyboard", 49.99);

            // Lägg till befintlig data i kalkylbladet (kommer att skjutas nedåt vid infogning)
            cells["A1"].PutValue("Existing Data");
            cells["A2"].PutValue(100);

            // Ställ in importalternativ med InsertRows = true
            ImportTableOptions options = new ImportTableOptions();
            options.InsertRows = true; // This will insert new rows instead of overwriting
            options.IsFieldNameShown = true;

            // Importera data med start på rad 1 (kommer att infoga rader under befintlig data)
            cells.ImportData(dataTable, 1, 0, options);

            // Spara arbetsboken
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


