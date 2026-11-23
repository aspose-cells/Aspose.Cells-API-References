---
title: "Classe ColorHelper"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.ColorHelper. Fournit des fonctions d'aide concernant la couleur"
type: docs
url: /fr/net/aspose.cells.drawing/colorhelper/
---
## ColorHelper class

Fournit des fonctions d'aide concernant la couleur.

```csharp
public class ColorHelper
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [FromOleColor](../../aspose.cells.drawing/colorhelper/fromolecolor/)(int) | Convertir OLE_COLOR. |
| static [ToOleColor](../../aspose.cells.drawing/colorhelper/toolecolor/)(Color, Workbook) | Convertir la couleur en OLE_COLOR |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassColorHelperDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Convertir la couleur OLE en System.Drawing.Color (Vert)
            int oleGreen = 0x00FF00;
            Color colorFromOle = ColorHelper.FromOleColor(oleGreen);

            // Appliquer la couleur convertie à l'arrière-plan de la cellule A1
            Cell cellA1 = worksheet.Cells["A1"];
            Style styleA1 = cellA1.GetStyle();
            styleA1.ForegroundColor = colorFromOle;
            styleA1.Pattern = BackgroundType.Solid;
            cellA1.SetStyle(styleA1);

            // Convertir System.Drawing.Color en couleur OLE
            int convertedOle = ColorHelper.ToOleColor(colorFromOle, workbook);

            // Convertir le résultat OLE en couleur (vérification)
            Color colorFromConvertedOle = ColorHelper.FromOleColor(convertedOle);

            // Appliquer la couleur reconvertie à l'arrière-plan de la cellule A2
            Cell cellA2 = worksheet.Cells["A2"];
            Style styleA2 = cellA2.GetStyle();
            styleA2.ForegroundColor = colorFromConvertedOle;
            styleA2.Pattern = BackgroundType.Solid;
            cellA2.SetStyle(styleA2);

            // Enregistrer le classeur modifié
            workbook.Save("DrawingClassColorHelperDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


