---
title: "PageSetup.CustomPaperSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit la taille personnalisée du papier en unités de pouces"
type: docs
url: /fr/net/aspose.cells/pagesetup/custompapersize/
---
## PageSetup.CustomPaperSize method

Définit la taille du papier personnalisé, en pouces.

```csharp
public void CustomPaperSize(double width, double height)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| largeur | Double | La largeur du papier. |
| hauteur | Double | La hauteur du papier. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCustomPaperSizeWithDoubleDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez la taille personnalisée du papier (largeur : 1,5 pouces, hauteur : 1,5 pouces)
            worksheet.PageSetup.CustomPaperSize(1.5, 1.5);
            
            // Enregistrez le classeur pour démontrer l'effet
            workbook.Save("CustomPaperSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


