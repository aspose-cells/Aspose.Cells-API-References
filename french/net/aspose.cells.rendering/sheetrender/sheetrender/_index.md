---
title: "SheetRender.SheetRender"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur SheetRender. la construction de SheetRender nécessite worksheet et ImageOrPrintOptions comme paramètres"
type: docs
url: /fr/net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

la construction de SheetRender, nécessite la feuille de calcul et ImageOrPrintOptions comme paramètres

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| worksheet | Feuille de calcul | Indiquez quelle feuille de calcul doit être rendue. |
| options | ImageOrPrintOptions | ImageOrPrintOptions contient certaines propriétés de l'image de sortie |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodCtorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Créez un classeur et ajoutez des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer des options d'image/impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;

            // Créez SheetRender avec Worksheet et ImageOrPrintOptions
            SheetRender render = new SheetRender(worksheet, options);

            // Afficher le nombre de pages
            Console.WriteLine("Page count: " + render.PageCount);

            // Enregistrez l'image rendue
            render.ToImage(0, "output.png");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


