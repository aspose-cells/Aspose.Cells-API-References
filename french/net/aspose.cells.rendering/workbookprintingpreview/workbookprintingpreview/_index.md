---
title: "WorkbookPrintingPreview.WorkbookPrintingPreview"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur WorkbookPrintingPreview. La construction de WorkbookPrintingPreview"
type: docs
url: /fr/net/aspose.cells.rendering/workbookprintingpreview/workbookprintingpreview/
---
## WorkbookPrintingPreview constructor

La construction de WorkbookPrintingPreview

```csharp
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| classeur | Classeur | Indiquez quel classeur doit être imprimé. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contient certaines propriétés de sortie |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewMethodCtorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Printing Preview");
            
            // Définissez les options d'impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Créez un aperçu d'impression avec le classeur et les options
            WorkbookPrintingPreview preview = new WorkbookPrintingPreview(workbook, options);
            
            // Affichez le nombre de pages
            Console.WriteLine("Total pages: " + preview.EvaluatedPageCount);
        }
    }
}
```

### Voir aussi

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


