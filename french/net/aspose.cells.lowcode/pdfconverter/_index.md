---
title: "Classe PdfConverter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.PdfConverter. Convertisseur pour convertir le fichier modèle en pdf"
type: docs
url: /fr/net/aspose.cells.lowcode/pdfconverter/
---
## PdfConverter class

Convertisseur pour convertir le fichier modèle en pdf.

```csharp
public class PdfConverter
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Convertit le fichier modèle en pdf |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process_1)(string, string) | Convertit le fichier modèle fourni en pdf. |

### Exemples

```csharp
using System;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassPdfConverterDemo
    {
        public static void Run()
        {
            // Initialiser le PdfConverter avec les chemins du modèle et de la sortie
            PdfConverter.Process("template.xlsx", "res.pdf");
            
            Console.WriteLine("PDF conversion completed successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


