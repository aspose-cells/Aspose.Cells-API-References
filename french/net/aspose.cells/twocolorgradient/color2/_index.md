---
title: "TwoColorGradient.Color2"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TwoColorGradient. Obtient et définit la deuxième couleur du dégradé"
type: docs
url: /fr/net/aspose.cells/twocolorgradient/color2/
---
## TwoColorGradient.Color2 property

Obtient et définit la deuxième couleur du dégradé.

```csharp
public Color Color2 { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor2Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de dégradé à deux couleurs
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.Green,
                GradientStyleType.Horizontal,
                1);

            // Créer le premier style avec le dégradé initial
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].PutValue("Initial Gradient");
            worksheet.Cells["A1"].SetStyle(style1);

            // Afficher la valeur actuelle de Color2
            System.Console.WriteLine("Current Color2: " + gradient.Color2);

            // Modifier la propriété Color2
            gradient.Color2 = Color.Red;

            // Créer le deuxième style avec le dégradé modifié
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A2"].PutValue("Modified Gradient");
            worksheet.Cells["A2"].SetStyle(style2);

            // Ajuster les lignes pour la visibilité
            worksheet.Cells.SetRowHeight(0, 40);
            worksheet.Cells.SetRowHeight(1, 40);

            // Enregistrez le classeur
            workbook.Save("TwoColorGradientColor2Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


