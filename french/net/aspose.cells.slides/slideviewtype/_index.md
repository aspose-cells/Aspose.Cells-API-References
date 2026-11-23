---
title: "Enum SlideViewType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Slides.SlideViewType enum. Représente le type lors de l'exportation vers des diapositives"
type: docs
url: /fr/net/aspose.cells.slides/slideviewtype/
---
## SlideViewType enumeration

Représente le type lors de l'exportation vers des diapositives.

```csharp
public enum SlideViewType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| View | `0` | Exportation en tant que vue dans MS Excel. |
| Print | `1` | Exportation en tant qu'impression. |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Slide 1 Content");
            worksheet.Cells["A2"].PutValue("This will appear in the exported slides");

            // Configurer les options d'enregistrement PPTX avec SlideViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                ExportViewType = SlideViewType.Print,
                OnePagePerSheet = true
            };

            // Enregistrer en PPTX
            workbook.Save("SlidesViewTypeDemo.pptx", saveOptions);
            
            Console.WriteLine("PPTX file created with SlideViewType.Print");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


