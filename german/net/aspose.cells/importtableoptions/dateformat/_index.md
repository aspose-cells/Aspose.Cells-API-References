---
title: "ImportTableOptions.DateFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Gibt das Datumsformat für Zellen mit importierten Datumszeitwerten zurück oder legt es fest"
type: docs
url: /de/net/aspose.cells/importtableoptions/dateformat/
---
## ImportTableOptions.DateFormat property

Liest oder legt das Datumsformat für Zellen mit importierten Datums‑Zeit‑Werten fest.

```csharp
public string DateFormat { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Beispiel-DataTable mit Datumswerten
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("DateColumn", typeof(DateTime));
            dataTable.Rows.Add(new DateTime(2023, 1, 15));
            dataTable.Rows.Add(new DateTime(2023, 2, 20));
            dataTable.Rows.Add(new DateTime(2023, 3, 25));

            // Definiere den Importbereich
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 10, 1);

            // Importiere Daten mit benutzerdefiniertem Datumsformat
            worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions()
            {
                IsFieldNameShown = true,
                DateFormat = "YYYY-MM-DD"
            });

            // Speichere die Arbeitsmappe, um das Ergebnis zu demonstrieren
            workbook.Save("DateFormatDemoOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


