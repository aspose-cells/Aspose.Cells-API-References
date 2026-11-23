---
title: "TwoColorGradient.Color1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TwoColorGradient. Obtient et définit la première couleur du dégradé"
type: docs
url: /fr/net/aspose.cells/twocolorgradient/color1/
---
## TwoColorGradient.Color1 property

Obtient et définit la première couleur du dégradé.

```csharp
public Color Color1 { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor1Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Créer un style avec remplissage en dégradé
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            // Initialiser le dégradé à deux couleurs
            style.SetTwoColorGradient(
                Color.Red,
                Color.Blue,
                GradientStyleType.Vertical,
                variant: 1);
            
            // Appliquer le dégradé au style de cellule
            cell.SetStyle(style);
            
            // Lire la couleur initiale
            TwoColorGradient gradient = style.GetTwoColorGradientSetting();
            Console.WriteLine("Current Color1 value: " + gradient.Color1);
            
            // Modifier la couleur du dégradé et réappliquer
            gradient.Color1 = Color.Lime;
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            
            // Vérifier la mise à jour
            Console.WriteLine("Updated Color1 value: " + gradient.Color1);
            
            // Démonstration visuelle dans le fichier de sortie
            cell.PutValue("Color1 Gradient Demo");
            worksheet.AutoFitColumn(0);
            workbook.Save("TwoColorGradientPropertyColor1Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


