---
title: "PptxSaveOptions.ExportViewType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PptxSaveOptions‑egenskap. Hämtar och anger visningstypen vid export till PowerPoint. Standardexporttypen fungerar som utskrift"
type: docs
url: /sv/net/aspose.cells/pptxsaveoptions/exportviewtype/
---
## PptxSaveOptions.ExportViewType property

Hämtar och anger visningstypen vid export till PowerPoint. Standardexporttypen fungerar som utskrift.

```csharp
public SlideViewType ExportViewType { get; set; }
```

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Ställ in PPTX‑sparalternativ med ExportViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.ExportViewType = SlideViewType.View;
            
            // Spara arbetsboken som PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved as PPTX with ExportViewType set to View");
        }
    }
}
```

### Se även

* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


