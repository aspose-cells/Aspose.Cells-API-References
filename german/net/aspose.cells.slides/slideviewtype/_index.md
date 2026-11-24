---
title: "Enum SlideViewType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Slides.SlideViewType enum. Stellt den Typ beim Exportieren zu Folien dar"
type: docs
url: /de/net/aspose.cells.slides/slideviewtype/
---
## SlideViewType enumeration

Stellt den Typ beim Exportieren zu Folien dar.

```csharp
public enum SlideViewType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| View | `0` | Exportieren als Ansicht in MS Excel. |
| Print | `1` | Exportieren als Druck. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Slide 1 Content");
            worksheet.Cells["A2"].PutValue("This will appear in the exported slides");

            // Konfiguriere PPTX-Speicheroptionen mit SlideViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                ExportViewType = SlideViewType.Print,
                OnePagePerSheet = true
            };

            // Speichern als PPTX
            workbook.Save("SlidesViewTypeDemo.pptx", saveOptions);
            
            Console.WriteLine("PPTX file created with SlideViewType.Print");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


