---
title: "MsoFillFormat.SetOneColorGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode MsoFillFormat. Définit le remplissage spécifié comme un dégradé à une couleur"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformat/setonecolorgradient/
---
## MsoFillFormat.SetOneColorGradient method

Définit le remplissage spécifié comme un dégradé d'une seule couleur.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color | Color | Une couleur de dégradé. |
| degré | Double | Le degré du dégradé. Peut être une valeur de 0.0 (sombre) à 1.0 (clair). |
| style | GradientStyleType | Style d’ombrage du dégradé. |
| variant | Int32 | La variante du dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes de l'onglet Dégradé dans la boîte de dialogue Effets de remplissage. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 50, 50);
            MsoFillFormat fillFormat = shape.FillFormat;

            // Définir un dégradé à une couleur avec les paramètres spécifiés
            fillFormat.SetOneColorGradient(Color.Red, 0.5, GradientStyleType.DiagonalUp, 2);

            workbook.Save("GradientFillExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


