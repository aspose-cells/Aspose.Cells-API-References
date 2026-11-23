---
title: "Classe MsoFillFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.MsoFillFormat. Représente le format de remplissage d'une forme"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformat/
---
## MsoFillFormat class

Représente le format de remplissage d'une forme.

```csharp
public class MsoFillFormat
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformat/backcolor/) { get; set; } | Obtient et définit la couleur d'arrière-plan du fichier. |
| [ForeColor](../../aspose.cells.drawing/msofillformat/forecolor/) { get; set; } | Obtient et définit la couleur de premier plan du remplissage. |
| [ImageData](../../aspose.cells.drawing/msofillformat/imagedata/) { get; set; } | Obtient et définit les données de remplissage Texture et Image. |
| [IsVisible](../../aspose.cells.drawing/msofillformat/isvisible/) { get; set; } | Indique s'il y a un remplissage. |
| [Texture](../../aspose.cells.drawing/msofillformat/texture/) { get; } | Obtient le type de remplissage de texture. |
| [Transparency](../../aspose.cells.drawing/msofillformat/transparency/) { get; set; } | Renvoie ou définit le degré de transparence du remplissage spécifié sous forme d'une valeur comprise entre 0.0 (opaque) et 1.0 (transparent). |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Définit le remplissage spécifié comme un dégradé d'une seule couleur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatDemo
    {
        public static void MsoFillFormatExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme d'arc à la feuille de calcul
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Accéder au format de remplissage de la forme
            MsoFillFormat fillFormat = arcShape.FillFormat;

            // Définir la couleur de premier plan du remplissage
            fillFormat.ForeColor = Color.Blue;

            // Définir la couleur d'arrière-plan du remplissage
            fillFormat.BackColor = Color.LightBlue;

            // Définir la transparence
            fillFormat.Transparency = 0.5;

            // Vérifier si le remplissage est visible
            bool isVisible = fillFormat.IsVisible;
            Console.WriteLine("Is Fill Visible: " + isVisible);

            // Définir un remplissage en dégradé à une couleur
            fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);

            // Enregistrez le classeur
            workbook.Save("MsoFillFormatExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


