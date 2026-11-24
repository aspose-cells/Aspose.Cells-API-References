---
title: "Range.ExportDataTableAsString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Exportiert die Daten dieses Bereichs in ein DataTable-Objekt"
type: docs
url: /de/net/aspose.cells/range/exportdatatableasstring/
---
## Range.ExportDataTableAsString method

Exportiert Daten dieses Bereichs in ein DataTable‑Objekt.

```csharp
public DataTable ExportDataTableAsString()
```

### Rückgabewert

Exportiertes DataTable-Objekt.

### Hinweise

Alle Daten in der [`Cells`](../../cells/) Sammlung werden in Zeichenfolgen konvertiert.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableAsStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(30);

            // Den Bereich mit Daten abrufen
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            try
            {
                // Rufen Sie die Methode ExportDataTableAsString auf
                DataTable dataTable = range.ExportDataTableAsString();

                // Zeige die exportierten Daten an
                Console.WriteLine("Exported DataTable:");
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}, {row[1]}");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("RangeMethodExportDataTableAsStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportDataTableAsString method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


