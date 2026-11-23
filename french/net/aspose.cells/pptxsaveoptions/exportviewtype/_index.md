---
title: "PptxSaveOptions.ExportViewType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PptxSaveOptions. Obtient et définit le type d'affichage lors de l'exportation vers PowerPoint. Le type d'exportation par défaut fonctionne comme l'impression"
type: docs
url: /fr/net/aspose.cells/pptxsaveoptions/exportviewtype/
---
## PptxSaveOptions.ExportViewType property

Obtient et définit le type d'affichage lors de l'exportation vers PowerPoint. Le type d'exportation par défaut fonctionne comme l'impression.

```csharp
public SlideViewType ExportViewType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyExportViewTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Définir les options d'enregistrement PPTX avec ExportViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.ExportViewType = SlideViewType.View;
            
            // Enregistrer le classeur au format PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved as PPTX with ExportViewType set to View");
        }
    }
}
```

### Voir aussi

* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


