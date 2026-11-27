---
title: "PptxSaveOptions.AdjustFontSizeForRowType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PptxSaveOptions-egenskap. Representerar vilken typ av rad som behöver justera teckenstorleken om radens höjd är liten"
type: docs
url: /sv/net/aspose.cells/pptxsaveoptions/adjustfontsizeforrowtype/
---
## PptxSaveOptions.AdjustFontSizeForRowType property

Representerar vilken typ av linje som behöver justera teckenstorleken om radens höjd är liten.

```csharp
public AdjustFontSizeForRowType AdjustFontSizeForRowType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data och tomma rader
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue(""); // Empty row
            worksheet.Cells["A4"].PutValue("Data 2");
            
            // Skapa PPTX-sparalternativ
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows;
            
            // Spara till PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("File saved with AdjustFontSizeForRowType setting");
        }
    }
}
```

### Se även

* enum [AdjustFontSizeForRowType](../../../aspose.cells.slides/adjustfontsizeforrowtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


