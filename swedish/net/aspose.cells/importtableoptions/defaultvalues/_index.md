---
title: "ImportTableOptions.DefaultValues"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions-egenskap. Standardvärdet för värdet i tabellen är null"
type: docs
url: /sv/net/aspose.cells/importtableoptions/defaultvalues/
---
## ImportTableOptions.DefaultValues property

Standardvärdet för värdet i tabellen är null.

```csharp
public object[] DefaultValues { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyDefaultValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata med nullvärden
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Quantity", typeof(int));
            dataTable.Columns.Add("ExpiryDate", typeof(DateTime));
            
            dataTable.Rows.Add("Bread", 10, DateTime.Now.AddDays(7));
            dataTable.Rows.Add(null, null, null); // Will use default values
            dataTable.Rows.Add("Milk", null, DateTime.Now.AddDays(3));

            ImportTableOptions importOptions = new ImportTableOptions();
            
            // Visa initialt tillstånd
            Console.WriteLine("Current DefaultValues: " + (importOptions.DefaultValues == null ? "Not set" : "Set"));

            // Konfigurera standardvärden för varje kolumn
            importOptions.DefaultValues = new object[] { "[Unspecified]", 1, DateTime.Today };

            // Importera data med nullhantering
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Autoanpassa kolumner för bättre synlighet
            worksheet.AutoFitColumns();

            workbook.Save("DefaultValuesDemo.xlsx");
            Console.WriteLine("Spreadsheet saved with default values applied to null entries.");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


