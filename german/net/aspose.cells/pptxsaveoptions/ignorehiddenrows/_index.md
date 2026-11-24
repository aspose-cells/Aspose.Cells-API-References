---
title: "PptxSaveOptions.IgnoreHiddenRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PptxSaveOptions-Eigenschaft. Gibt an, ob versteckte Zeilen beim Konvertieren von Excel zu PowerPoint ignoriert werden."
type: docs
url: /de/net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

Gibt an, ob versteckte Zeilen beim Konvertieren von Excel nach PowerPoint ignoriert werden.

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyIgnoreHiddenRowsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen und einige Zeilen ausblenden
            worksheet.Cells["A1"].PutValue("Visible Row 1");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row 2");
            
            // Zeile 2 ausblenden
            worksheet.Cells.Rows[1].IsHidden = true;

            // PPTX-Speicheroptionen mit IgnoreHiddenRows festlegen
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            
            // Speichern als PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("PPTX saved with hidden rows ignored.");
        }
    }
}
```

### Siehe auch

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


