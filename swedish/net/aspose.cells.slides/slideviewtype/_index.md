---
title: "Enum SlideViewType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Slides.SlideViewType enum. Representerar typen vid export till bilder"
type: docs
url: /sv/net/aspose.cells.slides/slideviewtype/
---
## SlideViewType enumeration

Representerar typen vid export till slides.

```csharp
public enum SlideViewType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| View | `0` | Exporterar som vy i MS Excel. |
| Print | `1` | Exporterar som utskrift. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassSlideViewTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Slide 1 Content");
            worksheet.Cells["A2"].PutValue("This will appear in the exported slides");

            // Konfigurera PPTX‑sparalternativ med SlideViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                ExportViewType = SlideViewType.Print,
                OnePagePerSheet = true
            };

            // Spara som PPTX
            workbook.Save("SlidesViewTypeDemo.pptx", saveOptions);
            
            Console.WriteLine("PPTX file created with SlideViewType.Print");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


