---
title: "HtmlSaveOptions.ExportHeadings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob Zeilen‑ und Spaltenüberschriften der Arbeitsblätter beim Speichern in HTML-Dateien exportiert werden."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportheadings/
---
## HtmlSaveOptions.ExportHeadings property

Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML-Dateien exportiert werden.

```csharp
[Obsolete("Use HtmlSaveOptions.ExportRowColumnHeadings instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExportHeadings { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die HtmlSaveOptions.ExportRowColumnHeadings‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Juni 2022, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHeadingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // HTML-Speicheroptionen erstellen und Exportüberschriften aktivieren
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportHeadings = true;

            // Als HTML mit Überschriften speichern
            workbook.Save("output_with_headings.html", options);
            
            // Erneut ohne Überschriften zum Vergleich speichern
            options.ExportHeadings = false;
            workbook.Save("output_without_headings.html", options);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


