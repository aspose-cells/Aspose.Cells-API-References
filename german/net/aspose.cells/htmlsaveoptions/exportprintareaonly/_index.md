---
title: "HtmlSaveOptions.ExportPrintAreaOnly"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob nur der Druckbereich in die HTML-Datei exportiert wird. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportprintareaonly/
---
## HtmlSaveOptions.ExportPrintAreaOnly property

Gibt an, ob nur der Druckbereich in eine html-Datei exportiert wird. Der Standardwert ist false.

```csharp
public bool ExportPrintAreaOnly { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPrintAreaOnlyDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten festlegen
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Druckbereich festlegen
            worksheet.PageSetup.PrintArea = "B2:F10";

            // HTML-Speicheroptionen konfigurieren
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportPrintAreaOnly = true;
            options.ExportGridLines = true;

            // Arbeitsmappe nur mit Druckbereich speichern
            workbook.Save("output.html", options);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


