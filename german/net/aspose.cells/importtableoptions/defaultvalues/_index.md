---
title: "ImportTableOptions.DefaultValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Standardwert für den Wert in der Tabelle ist null"
type: docs
url: /de/net/aspose.cells/importtableoptions/defaultvalues/
---
## ImportTableOptions.DefaultValues property

Der Standardwert für den Wert in der Tabelle ist null.

```csharp
public object[] DefaultValues { get; set; }
```

### Beispiele

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

            // Erstelle Beispieldaten mit Nullwerten
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Quantity", typeof(int));
            dataTable.Columns.Add("ExpiryDate", typeof(DateTime));
            
            dataTable.Rows.Add("Bread", 10, DateTime.Now.AddDays(7));
            dataTable.Rows.Add(null, null, null); // Will use default values
            dataTable.Rows.Add("Milk", null, DateTime.Now.AddDays(3));

            ImportTableOptions importOptions = new ImportTableOptions();
            
            // Zeige den Anfangszustand an
            Console.WriteLine("Current DefaultValues: " + (importOptions.DefaultValues == null ? "Not set" : "Set"));

            // Konfiguriere Standardwerte für jede Spalte
            importOptions.DefaultValues = new object[] { "[Unspecified]", 1, DateTime.Today };

            // Importiere Daten mit Nullwertbehandlung
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Spalten automatisch anpassen für bessere Sichtbarkeit
            worksheet.AutoFitColumns();

            workbook.Save("DefaultValuesDemo.xlsx");
            Console.WriteLine("Spreadsheet saved with default values applied to null entries.");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


