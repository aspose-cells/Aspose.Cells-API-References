---
title: "PptxSaveOptions.IgnoreHiddenRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PptxSaveOptions-egenskap. Anger om dolda rader ska ignoreras vid konvertering av Excel till PowerPoint"
type: docs
url: /sv/net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

Indikerar om dolda rader ska ignoreras vid konvertering från Excel till PowerPoint.

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyIgnoreHiddenRowsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och dölj några rader
            worksheet.Cells["A1"].PutValue("Visible Row 1");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row 2");
            
            // Dölj rad 2
            worksheet.Cells.Rows[1].IsHidden = true;

            // Ställ in PPTX-sparalternativ med IgnoreHiddenRows
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            
            // Spara som PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("PPTX saved with hidden rows ignored.");
        }
    }
}
```

### Se även

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


