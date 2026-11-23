---
title: "WorkbookRender.GetPageSizeInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorkbookRender. Obtient la taille de la page en pouces de l'image de sortie"
type: docs
url: /fr/net/aspose.cells.rendering/workbookrender/getpagesizeinch/
---
## WorkbookRender.GetPageSizeInch method

Obtenir la taille de page en pouces de l’image de sortie.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de la page est basé sur zéro. |

### Valeur de retour

Taille de l'image, [0] pour la largeur et [1] pour la hauteur

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test page size");
            sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            WorkbookRender wr = new WorkbookRender(wb, imgOpt);
            
            float[] pageSize = wr.GetPageSizeInch(0);
            Console.WriteLine($"Page size in inches: {pageSize[0]} x {pageSize[1]}");
        }
    }
}
```

### Voir aussi

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


