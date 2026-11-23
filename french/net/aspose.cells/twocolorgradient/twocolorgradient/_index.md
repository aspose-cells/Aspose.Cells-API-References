---
title: "TwoColorGradient.TwoColorGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur TwoColorGradient."
type: docs
url: /fr/net/aspose.cells/twocolorgradient/twocolorgradient/
---
## TwoColorGradient constructor

```csharp
public TwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color1 | Color |  |
| color2 | Color |  |
| gradientStyleType | GradientStyleType |  |
| variant | Int32 |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class TwoColorGradientMethodSharpctorWithColorColorGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Créer une instance de TwoColorGradient en utilisant le constructeur avec tous les paramètres
                TwoColorGradient gradient = new TwoColorGradient(
                    Color.LightBlue,
                    Color.DarkBlue,
                    GradientStyleType.Horizontal,
                    1);

                // Afficher les propriétés du dégradé pour vérifier l'initialisation
                Console.WriteLine($"Gradient created with:");
                Console.WriteLine($"Color1: {gradient.Color1}");
                Console.WriteLine($"Color2: {gradient.Color2}");
                Console.WriteLine($"GradientStyleType: {gradient.GradientStyleType}");
                Console.WriteLine($"Variant: {gradient.Variant}");

                // Créer un classeur et appliquer le dégradé pour démontrer la fonctionnalité
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Appliquer le dégradé à une cellule
                Style style = workbook.CreateStyle();
                style.SetTwoColorGradient(
                    gradient.Color1,
                    gradient.Color2,
                    gradient.GradientStyleType,
                    gradient.Variant);

                worksheet.Cells["A1"].PutValue("TwoColorGradient Demo");
                worksheet.Cells["A1"].SetStyle(style);

                // Enregistrez le classeur
                workbook.Save("TwoColorGradientDemo.xlsx");
                Console.WriteLine("Gradient applied successfully to workbook.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


