---
title: "HtmlSaveOptions.ExportExtraHeadings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger ist als die maximal anzuzeigende Spalte. Der Standardwert ist false. Wenn Sie die html-Datei nach excel importieren möchten, behalten Sie bitte den Standardwert bei."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportextraheadings/
---
## HtmlSaveOptions.ExportExtraHeadings property

Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger ist als die maximal anzuzeigende Spalte. Der Standardwert ist false. Wenn Sie die html-Datei in excel importieren möchten, belassen Sie bitte den Standardwert.

```csharp
public bool ExportExtraHeadings { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportExtraHeadingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und zusätzliche Überschriften hinzufügen
            worksheet.Cells["A1"].PutValue("Main Heading");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");
            
            // Zusätzliche Überschriften festlegen (Zeilen und Spalten)
            worksheet.Cells["Z1"].PutValue("Extra Column Heading");
            worksheet.Cells["A100"].PutValue("Extra Row Heading");

            // HTML-Speicheroptionen mit ExportExtraHeadings konfigurieren
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportHeadings = true;
            saveOptions.ExportExtraHeadings = true;

            // Als HTML speichern
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML exported with extra headings.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


