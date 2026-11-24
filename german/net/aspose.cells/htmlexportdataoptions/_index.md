---
title: "Enum HtmlExportDataOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlExportDataOptions Enum. Stellt die Optionen für den Export von HTML‑Daten dar."
type: docs
url: /de/net/aspose.cells/htmlexportdataoptions/
---
## HtmlExportDataOptions enumeration

Stellt die Optionen für den Export von HTML‑Daten dar.

```csharp
public enum HtmlExportDataOptions
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Table | `1` | Exportieren Sie die Datei nach HTML, die nur den Tabellenteil enthält. |
| All | `255` | Exportieren Sie alle Daten nach HTML. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlExportDataOptionsDemo
    {
        public static void HtmlExportDataOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Doe");
            worksheet.Cells["B3"].PutValue(25);

            // Erstellen Sie HtmlSaveOptions und setzen Sie die HtmlExportDataOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All; // Export all data to HTML

            // Speichere das Arbeitsbuch im HTML‑Format
            workbook.Save("HtmlExportDataOptionsExample_All.html", saveOptions);

            // Ändern Sie die HtmlExportDataOptions, um nur den Tabellenteil zu exportieren
            saveOptions.ExportDataOptions = HtmlExportDataOptions.Table; // Export only the table part

            // Speichern Sie das Arbeitsbuch erneut im HTML-Format
            workbook.Save("HtmlExportDataOptionsExample_Table.html", saveOptions);

            Console.WriteLine("HTML files have been saved successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


