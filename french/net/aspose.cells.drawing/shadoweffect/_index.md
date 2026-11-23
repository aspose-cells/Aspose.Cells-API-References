---
title: "Classe ShadowEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ShadowEffect class. Cette classe spécifie l'effet d'ombre de l'élément de graphique ou de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shadoweffect/
---
## ShadowEffect class

Cette classe spécifie l'effet d'ombre de l'élément de graphique ou de la forme.

```csharp
public class ShadowEffect
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Angle](../../aspose.cells.drawing/shadoweffect/angle/) { get; set; } | Obtient et définit l'angle d'éclairage. Plage de 0 à 359,9 degrés. |
| [Blur](../../aspose.cells.drawing/shadoweffect/blur/) { get; set; } | Obtient et définit le flou de l'ombre. Plage de 0 à 100 points. |
| [Color](../../aspose.cells.drawing/shadoweffect/color/) { get; set; } | Obtient et définit la couleur de l'ombre. |
| [Distance](../../aspose.cells.drawing/shadoweffect/distance/) { get; set; } | Obtient et définit la distance de l'ombre. Plage de 0 à 200 points. |
| [PresetType](../../aspose.cells.drawing/shadoweffect/presettype/) { get; set; } | Obtient et définit le type d'ombre prédéfini de l'ombre. |
| [Size](../../aspose.cells.drawing/shadoweffect/size/) { get; set; } | Obtient et définit la taille de l'ombre. Plage de 0 à 2,0. Sans effet dans l'ombre interne. |
| [Transparency](../../aspose.cells.drawing/shadoweffect/transparency/) { get; set; } | Obtient et définit le degré de transparence de l'ombre. Plage de 0,0 (opaque) à 1,0 (transparent). |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShadowEffectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Obtenir l'effet d'ombre de la forme
            ShadowEffect shadow = shape.ShadowEffect;

            // Définir les propriétés de l'ombre
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            Console.WriteLine("Shadow effect demo completed successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


