---
title: "Enum PdfFontEncoding"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Rendering.PdfFontEncoding enum. Représente l'encodage des polices intégrées au PDF"
type: docs
url: /fr/net/aspose.cells.rendering/pdffontencoding/
---
## PdfFontEncoding enumeration

Représente le codage de police intégré pdf.

```csharp
public enum PdfFontEncoding
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Identity | `0` | Représente l'utilisation de l'encodage Identity-H pour toutes les polices intégrées dans le PDF. |
| AnsiPrefer | `1` | Représente la préférence d'utiliser WinAnsiEncoding pour les polices TrueType avec les caractères 32-127, sinon, l'encodage Identity-H sera utilisé pour les polices intégrées dans le PDF. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfFontEncodingDemo
    {
        public static void PdfFontEncodingExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");

            // Créez PdfSaveOptions et définissez la propriété FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;

            // Enregistrer le classeur au format PDF
            workbook.Save("PdfFontEncodingExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file created successfully with specified font encoding.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


