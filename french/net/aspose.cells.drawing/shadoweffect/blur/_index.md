---
title: "ShadowEffect.Blur"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShadowEffect. Obtient et définit le flou de l'ombre. Plage de 0 à 100 points"
type: docs
url: /fr/net/aspose.cells.drawing/shadoweffect/blur/
---
## ShadowEffect.Blur property

Obtient et définit le flou de l'ombre. Plage de 0 à 100 points.

```csharp
public double Blur { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme d'exemple
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Obtenir l'effet d'ombre
            ShadowEffect shadow = shape.ShadowEffect;
            
            // Définir les propriétés de l'ombre, y compris le flou
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Shadow effect with blur applied successfully.");
        }
    }
}
```

### Voir aussi

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


