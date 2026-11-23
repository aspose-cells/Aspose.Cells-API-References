---
title: "WorkbookRender.WorkbookRender"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur WorkbookRender. La construction de WorkbookRender"
type: docs
url: /fr/net/aspose.cells.rendering/workbookrender/workbookrender/
---
## WorkbookRender constructor

La construction de WorkbookRender

```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| classeur | Classeur | Indiquer quel classeur doit être rendu. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contient certaines propriétés de l'image de sortie |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodctorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Créer des options d'image/impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Créer le rendu du classeur
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            
            // Afficher le nombre de pages
            Console.WriteLine("Total pages: " + renderer.PageCount);
        }
    }
}
```

### Voir aussi

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


