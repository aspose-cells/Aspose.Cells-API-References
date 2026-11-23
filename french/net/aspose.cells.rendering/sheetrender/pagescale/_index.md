---
title: "SheetRender.PageScale"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SheetRender. Obtient l'échelle de page calculée de la feuille. Retourne l'échelle définie si Zoom est défini. Sinon, retourne l'échelle calculée selon FitToPagesWide et FitToPagesTall"
type: docs
url: /fr/net/aspose.cells.rendering/sheetrender/pagescale/
---
## SheetRender.PageScale property

Obtient l'échelle de page calculée de la feuille. Retourne l'échelle définie si [`Zoom`](../../../aspose.cells/pagesetup/zoom/) est défini. Sinon, retourne l'échelle calculée selon [`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide/) et [`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall/).

```csharp
public double PageScale { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageScaleDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue($"Item {i + 1}");
                sheet.Cells[i, 1].PutValue((i + 1) * 10);
            }

            // Créer des options d'image ou d'impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Créer un rendu de feuille
            SheetRender sheetRender = new SheetRender(sheet, options);
            
            // Obtenir et afficher l'échelle de page calculée
            double pageScale = sheetRender.PageScale;
            Console.WriteLine($"Calculated Page Scale: {pageScale}");
        }
    }
}
```

### Voir aussi

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


