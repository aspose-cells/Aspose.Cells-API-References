---
title: "FillFormat.SetOneColorGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FillFormat. Définit le remplissage spécifié à un dégradé à une couleur. Ne s'applique que pour Excel 2007"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/setonecolorgradient/
---
## FillFormat.SetOneColorGradient method

Définit le remplissage spécifié comme un dégradé à une couleur. S'applique uniquement à Excel 2007.

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
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Appliquer le remplissage en dégradé à la première série
            Series series = chart.NSeries[0];
            series.IsColorVaried = false;
            
            // Démontrer SetOneColorGradient avec des paramètres spécifiques
            series.Area.FillFormat.SetOneColorGradient(
                Color.FromArgb(0, 236, 102, 102), // Color
                0.9,                              // Transparency
                Aspose.Cells.Drawing.GradientStyleType.DiagonalDown,    // Gradient style
                2);                                // Variant

            // Enregistrez le classeur
            workbook.Save("FillFormat_SetOneColorGradient_Output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


