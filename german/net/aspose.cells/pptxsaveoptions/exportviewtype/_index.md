---
title: "PptxSaveOptions.ExportViewType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PptxSaveOptions-Eigenschaft. Gibt den Anzeigetyp beim Exportieren nach PowerPoint zurück und setzt ihn. Der standardmäßige Exporttyp funktioniert wie ein Druckvorgang."
type: docs
url: /de/net/aspose.cells/pptxsaveoptions/exportviewtype/
---
## PptxSaveOptions.ExportViewType property

Liest und setzt den Anzeigetyp beim Exportieren nach PowerPoint. Der standardmäßige Exporttyp funktioniert wie beim Drucken.

```csharp
public SlideViewType ExportViewType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyExportViewTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Setze PPTX-Speicheroptionen mit ExportViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.ExportViewType = SlideViewType.View;
            
            // Speichere die Arbeitsmappe als PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved as PPTX with ExportViewType set to View");
        }
    }
}
```

### Siehe auch

* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


