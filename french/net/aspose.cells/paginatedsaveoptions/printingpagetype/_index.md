---
title: "PaginatedSaveOptions.PrintingPageType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Indique quelles pages ne seront pas imprimées"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/printingpagetype/
---
## PaginatedSaveOptions.PrintingPageType property

Indique quelles pages ne seront pas imprimées.

```csharp
public PrintingPageType PrintingPageType { get; set; }
```

### Remarques

Si le contenu de la feuille est clairsemé, certaines pages seront totalement vides dans le fichier PDF de sortie. Si vous ne voulez pas de ces pages blanches, vous pouvez utiliser cette option pour les omettre.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPrintingPageTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123);
            ws.Cells["A3"].PutValue(456);
            
            // Créer une feuille de calcul vierge
            Worksheet blankWs = wb.Worksheets.Add("BlankSheet");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Enregistrer en ignorant les pages blanches
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            wb.Save("output_ignore_blank_page.pdf", pdfSaveOptions);
            
            // Enregistrer en ignorant les pages blanches et les pages contenant uniquement du style
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;
            wb.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* enum [PrintingPageType](../../printingpagetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


