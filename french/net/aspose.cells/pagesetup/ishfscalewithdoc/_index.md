---
title: "PageSetup.IsHFScaleWithDoc"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Indique si l'en-tête et le pied de page sont mis à l'échelle avec le redimensionnement du document. S'applique uniquement à Excel 2007."
type: docs
url: /fr/net/aspose.cells/pagesetup/ishfscalewithdoc/
---
## PageSetup.IsHFScaleWithDoc property

Indique si l'en-tête et le pied de page sont mis à l'échelle avec le redimensionnement du document. S'applique uniquement à Excel 2007.

```csharp
public bool IsHFScaleWithDoc { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFScaleWithDocDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Définissez la configuration de page de base.
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;

            // Démontrez la propriété IsHFScaleWithDoc.
            pageSetup.IsHFScaleWithDoc = true;
            Console.WriteLine("Header/Footer scaling with document is set to: " + pageSetup.IsHFScaleWithDoc);

            // Enregistrez le classeur
            workbook.Save("PageSetup_IsHFScaleWithDoc_Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


