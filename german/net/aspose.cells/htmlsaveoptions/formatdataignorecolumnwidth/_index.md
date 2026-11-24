---
title: "HtmlSaveOptions.FormatDataIgnoreColumnWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob die gesamten formatierten Daten einer Zelle angezeigt werden sollen, wenn sie die Spalte überlaufen. Wenn true, wird die Spaltenbreite ignoriert und die gesamten Zellen­daten werden exportiert. Wenn false, werden die Daten wie in Excel exportiert. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/
---
## HtmlSaveOptions.FormatDataIgnoreColumnWidth property

Gibt an, ob die gesamten formatierten Daten einer Zelle angezeigt werden sollen, wenn sie die Spalte überläuft. Wenn true, wird die Spaltenbreite ignoriert und die gesamten Zellen­daten werden exportiert. Wenn false, werden die Daten wie in Excel exportiert. Der Standardwert ist false.

```csharp
public bool FormatDataIgnoreColumnWidth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFormatDataIgnoreColumnWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und Spaltenbreite festlegen
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B1"].PutValue("Longer Text That Might Be Truncated");
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 5);  // Very narrow column

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Demonstriere die FormatDataIgnoreColumnWidth‑Eigenschaft
            saveOptions.FormatDataIgnoreColumnWidth = true; // Text won't be truncated by column width
            
            // Speichere mit verschiedenen Einstellungen, um die Wirkung zu zeigen
            workbook.Save("HtmlWithIgnoreColumnWidth.html", saveOptions);
            
            saveOptions.FormatDataIgnoreColumnWidth = false; // Text may be truncated by column width
            workbook.Save("HtmlWithoutIgnoreColumnWidth.html", saveOptions);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


