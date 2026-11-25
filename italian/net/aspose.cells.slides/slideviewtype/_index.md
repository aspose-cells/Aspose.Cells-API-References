---
title: "Enum SlideViewType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Slides.SlideViewType enum. Rappresenta il tipo durante l'esportazione in diapositive"
type: docs
url: /it/net/aspose.cells.slides/slideviewtype/
---
## SlideViewType enumeration

Rappresenta il tipo durante l'esportazione in diapositive.

```csharp
public enum SlideViewType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| View | `0` | Esportazione come visualizzazione in MS Excel. |
| Print | `1` | Esportazione come stampa. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Slide 1 Content");
            worksheet.Cells["A2"].PutValue("This will appear in the exported slides");

            // Configura le opzioni di salvataggio PPTX con SlideViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                ExportViewType = SlideViewType.Print,
                OnePagePerSheet = true
            };

            // Salva come PPTX
            workbook.Save("SlidesViewTypeDemo.pptx", saveOptions);
            
            Console.WriteLine("PPTX file created with SlideViewType.Print");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


