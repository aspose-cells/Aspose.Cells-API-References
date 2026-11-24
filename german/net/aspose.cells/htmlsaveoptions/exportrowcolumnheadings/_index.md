---
title: "HtmlSaveOptions.ExportRowColumnHeadings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob Zeilen‑ und Spaltenüberschriften der Arbeitsblätter beim Speichern in HTML-Dateien exportiert werden."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportrowcolumnheadings/
---
## HtmlSaveOptions.ExportRowColumnHeadings property

Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML-Dateien exportiert werden.

```csharp
public bool ExportRowColumnHeadings { get; set; }
```

### Hinweise

Der Standardwert ist false.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportRowColumnHeadingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Setzen Sie ExportRowColumnHeadings auf false (Standard ist true)
            saveOptions.ExportRowColumnHeadings = false;

            // Speichern Sie die Arbeitsmappe mit deaktivierten Überschriften
            workbook.Save("output_without_headings.html", saveOptions);

            // Aktivieren Sie jetzt die Überschriften und speichern Sie erneut
            saveOptions.ExportRowColumnHeadings = true;
            workbook.Save("output_with_headings.html", saveOptions);

            Console.WriteLine("HTML files saved with different heading visibility settings.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


