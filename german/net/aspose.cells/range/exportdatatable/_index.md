---
title: "Range.ExportDataTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Exportiert die Daten dieses Bereichs in ein DataTable-Objekt"
type: docs
url: /de/net/aspose.cells/range/exportdatatable/
---
## ExportDataTable() {#exportdatatable}

Exportiert Daten dieses Bereichs in ein DataTable‑Objekt.

```csharp
public DataTable ExportDataTable()
```

### Rückgabewert

Exportiertes DataTable-Objekt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten im Arbeitsblatt erstellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(450.75);

            // Erstelle einen Bereich, der die Daten enthält
            Aspose.Cells.Range dataRange = worksheet.Cells.CreateRange("A1:B4");

            try
            {
                // Exportiere den Bereich in ein DataTable
                DataTable dataTable = dataRange.ExportDataTable();

                Console.WriteLine("Data exported successfully to DataTable");
                Console.WriteLine($"DataTable contains {dataTable.Rows.Count} rows and {dataTable.Columns.Count} columns");

                // Zeige die exportierten Daten an
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}: {row[1]}");
                }

                // Modifiziere das DataTable und importiere es bei Bedarf zurück
                dataTable.Rows[0]["Price"] = 1300.00;
                Console.WriteLine("\nModified first product price in DataTable to 1300.00");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error exporting data: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RangeMethodExportDataTableDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(ExportTableOptions) {#exportdatatable_1}

Exportiert Daten dieses Bereichs in ein DataTable‑Objekt.

```csharp
public DataTable ExportDataTable(ExportTableOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | ExportTableOptions | Die Optionen zum Exportieren des Bereichs in ein DataTable. |

### Rückgabewert

Exportiertes DataTable-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class RangeMethodExportDataTableWithExportTableOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten im Arbeitsblatt erstellen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Benenne den Bereich, der unsere Daten enthält
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1:B3");
            namedRange.Name = "Names";

            // Exportiere den benannten Bereich mit Optionen in ein DataTable
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            DataTable dataTable = namedRange.ExportDataTable(options);

            // Ergebnisse anzeigen
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
            }
        }
    }
}
```

### Siehe auch

* class [ExportTableOptions](../../exporttableoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


