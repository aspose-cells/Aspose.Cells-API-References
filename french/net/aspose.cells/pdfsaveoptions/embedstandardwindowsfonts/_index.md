---
title: "PdfSaveOptions.EmbedStandardWindowsFonts"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PdfSaveOptions property. Vrai pour incorporer les polices TrueType. Affecte uniquement les caractères ASCII 32127. Les polices pour les codes de caractères supérieurs à 127 sont toujours incorporées. Les polices sont toujours incorporées pour les normes PDF/A1a PDF/A1b. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/
---
## PdfSaveOptions.EmbedStandardWindowsFonts property

True pour intégrer les polices TrueType. N'affecte que les caractères ASCII 32-127. Les polices pour les codes de caractères supérieurs à 127 sont toujours intégrées. Les polices sont toujours intégrées pour les normes PDF/A-1a, PDF/A-1b. La valeur par défaut est true.

```csharp
public bool EmbedStandardWindowsFonts { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedStandardWindowsFontsDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF with embedded fonts");

            // Définir les options d'enregistrement PDF avec la propriété EmbedStandardWindowsFonts
            PdfSaveOptions options = new PdfSaveOptions();
            options.EmbedStandardWindowsFonts = true;

            // Enregistrer dans le flux mémoire
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved with embedded fonts: " + (ms.Length > 0));
            }

            // Démontrer la désactivation de l'incorporation des polices
            options.EmbedStandardWindowsFonts = false;
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved without embedded fonts: " + (ms.Length > 0));
            }
        }
    }
}
```

### Voir aussi

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


