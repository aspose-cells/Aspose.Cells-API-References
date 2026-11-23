---
title: "Enum PrintingPageType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.PrintingPageType enum. Indique quelles pages ne seront pas imprimées"
type: docs
url: /fr/net/aspose.cells/printingpagetype/
---
## PrintingPageType enumeration

Indique quelles pages ne seront pas imprimées.

```csharp
public enum PrintingPageType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | Imprime toutes les pages. |
| IgnoreBlank | `1` | Ne pas imprimer les pages dont les cellules sont vides. |
| IgnoreStyle | `2` | Ne pas imprimer les pages dont les cellules ne contiennent que des styles. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintingPageTypeDemo
    {
        public static void PrintingPageTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques données dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("!");

            // Créer PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Définir PrintingPageType sur IgnoreBlank
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;

            // Enregistrez le classeur au format PDF avec les options spécifiées
            workbook.Save("output_ignore_blank_page.pdf", pdfSaveOptions);

            // Définir PrintingPageType sur IgnoreStyle
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;

            // Enregistrez le classeur au format PDF avec les options spécifiées
            workbook.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);

            // Définir PrintingPageType sur Default
            pdfSaveOptions.PrintingPageType = PrintingPageType.Default;

            // Enregistrez le classeur au format PDF avec les options spécifiées
            workbook.Save("output_default_page.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


