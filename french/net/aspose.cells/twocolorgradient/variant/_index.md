---
title: "TwoColorGradient.Variant"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TwoColorGradient. Obtient et définit la variante du dégradé"
type: docs
url: /fr/net/aspose.cells/twocolorgradient/variant/
---
## TwoColorGradient.Variant property

Obtient et définit la variante du dégradé.

```csharp
public int Variant { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un dégradé bicolore avec la variante initiale
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.DarkBlue,
                GradientStyleType.Horizontal,
                1
            );

            // Créer et appliquer le style à la cellule A1
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Variant 1");

            // Afficher la valeur actuelle de la variante
            System.Console.WriteLine("Current Variant value: " + gradient.Variant);

            // Modifier la valeur de la variante
            gradient.Variant = 2;

            // Créer et appliquer le style modifié à la cellule B1
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Variant 2");

            // Rendre les cellules plus hautes pour visualiser les dégradés
            worksheet.Cells.Rows[0].Height = 150;

            workbook.Save("TwoColorGradientVariantDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


