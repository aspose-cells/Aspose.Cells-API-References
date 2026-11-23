---
title: "ShadowEffect.Size"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShadowEffect. Obtient et définit la taille de l'ombre. Plage de 0 à 2,0. Sans signification dans l'ombre interne"
type: docs
url: /fr/net/aspose.cells.drawing/shadoweffect/size/
---
## ShadowEffect.Size property

Obtient et définit la taille de l'ombre. Plage de 0 à 2,0. Sans effet dans l'ombre interne.

```csharp
public double Size { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook book = new Workbook();
            
            // Accéder à la première feuille de calcul et ajouter une forme
            Worksheet sheet = book.Worksheets[0];
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Obtenir l'effet d'ombre et définir les propriétés, y compris la taille
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3; // Demonstrating Size property usage
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Enregistrez le classeur
            book.Save("ShadowEffectExample.xlsx");
            
            Console.WriteLine("Shadow effect with Size property set to 1.3 has been applied.");
        }
    }
}
```

### Voir aussi

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


