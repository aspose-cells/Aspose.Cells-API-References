---
title: "ExportTableOptions.CheckMixedValueType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportTableOptions‑Eigenschaft. False: Aspose.Cells setzt den Typ der DataColumns anhand des Wertetyps der ersten Zeile für die Leistung. True: Aspose.Cells prüft, ob die Wertetypen in der Spalte gemischt sind, bevor der Typ der DataColumns festgelegt wird. Sind die Wertetypen gemischt, wird der Typ der DataColumns zu string."
type: docs
url: /de/net/aspose.cells/exporttableoptions/checkmixedvaluetype/
---
## ExportTableOptions.CheckMixedValueType property

False: Aspose.Cells setzt den Typ der DataColumn anhand des Wertetyps der ersten Zeile aus Performance‑Gründen. True: Aspose.Cells prüft, ob der Wertetyp in der Spalte gemischt ist, bevor der Typ der DataColumn festgelegt wird. Ist der Wertetyp gemischt, wird der Typ der DataColumn zu string.

```csharp
public bool CheckMixedValueType { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyCheckMixedValueTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kopfzeilen hinzufügen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value Date");

            // Beispieldaten mit gemischten Typen hinzufügen
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue("2023-01-15");
            worksheet.Cells["A4"].PutValue("3");
            worksheet.Cells["B4"].PutValue(DateTime.Now.AddDays(1));

            // Exportoptionen mit aktiviertem CheckMixedValueType erstellen
            ExportTableOptions options = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true
            };

            // Daten in DataTable exportieren
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 2, options);

            // Ergebnisse anzeigen
            Console.WriteLine("Columns: " + dataTable.Columns.Count);
            Console.WriteLine("Rows: " + dataTable.Rows.Count);
            Console.WriteLine("ID column type: " + dataTable.Columns["ID"].DataType);
            Console.WriteLine("Value Date column type: " + dataTable.Columns["Value Date"].DataType);
        }
    }
}
```

### Siehe auch

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


