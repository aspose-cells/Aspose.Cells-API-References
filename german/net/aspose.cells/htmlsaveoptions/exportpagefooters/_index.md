---
title: "HtmlSaveOptions.ExportPageFooters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob Seitenköpfe exportiert werden"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportpagefooters/
---
## HtmlSaveOptions.ExportPageFooters property

Gibt an, ob Seitenköpfe exportiert werden.

```csharp
public bool ExportPageFooters { get; set; }
```

### Hinweise

Funktioniert nur, wenn [`SaveAsSingleFile`](../saveassinglefile/) True ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageFootersDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Setze ExportPageFooters auf true, um Seitenfußzeilen in die Ausgabe einzuschließen
            saveOptions.ExportPageFooters = true;
            
            // Weitere notwendige Optionen festlegen
            saveOptions.ExportPageHeaders = true;
            
            // Arbeitsmappe nach HTML speichern
            workbook.Save("HtmlWithPageFooters.html", saveOptions);
            
            Console.WriteLine("HTML file with page footers exported successfully.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


