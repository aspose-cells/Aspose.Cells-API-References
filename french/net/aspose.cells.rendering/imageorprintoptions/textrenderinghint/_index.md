---
title: "ImageOrPrintOptions.TextRenderingHint"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Spécifie la qualité du rendu du texte. La valeur par défaut est TextRenderingHint.SystemDefault"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/textrenderinghint/
---
## ImageOrPrintOptions.TextRenderingHint property

Spécifie la qualité du rendu du texte. La valeur par défaut est TextRenderingHint.SystemDefault

```csharp
public TextRenderingHint TextRenderingHint { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTextRenderingHintDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du texte d'exemple pour démontrer le rendu du texte
            worksheet.Cells["A1"].PutValue("Text Rendering Hint Demo");
            
            HtmlSaveOptions options = new HtmlSaveOptions();
#if !NETCOREAPP3_1_OR_GREATER
            options.ImageOptions.TextRenderingHint = TextRenderingHint.AntiAlias;
#endif
            workbook.Save("output.html", options);
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


