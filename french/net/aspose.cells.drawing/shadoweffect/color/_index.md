---
title: "ShadowEffect.Color"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShadowEffect. Obtient et définit la couleur de l’ombre"
type: docs
url: /fr/net/aspose.cells.drawing/shadoweffect/color/
---
## ShadowEffect.Color property

Obtient et définit la couleur de l'ombre.

```csharp
public CellsColor Color { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShadowEffectPropertyColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire pour démontrer l’effet d’ombre
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Obtenir l’effet d’ombre de la forme
                ShadowEffect shadowEffect = shape.ShadowEffect;

                // Créer un nouvel objet CellsColor
                CellsColor shadowColor = workbook.CreateCellsColor();

                // Définir la couleur en rouge en utilisant les valeurs RVB
                shadowColor.Color = Color.Red;

                // Appliquer la couleur à l’effet d’ombre
                shadowEffect.Color = shadowColor;

                // Afficher la valeur actuelle de la couleur
                Console.WriteLine("Shadow Color (RGB): " + shadowEffect.Color.Color.ToString());
                Console.WriteLine("Shadow Color (ARGB): " + shadowEffect.Color.Argb);

                // Enregistrez le classeur pour démontrer l'effet
                workbook.Save("ShadowEffectColorDemo.xlsx");

                // Charger à nouveau le classeur pour vérifier que la couleur a été enregistrée
                Workbook loadedWorkbook = new Workbook("ShadowEffectColorDemo.xlsx");
                ShadowEffect loadedShadowEffect = loadedWorkbook.Worksheets[0].Shapes[0].ShadowEffect;

                // Afficher la valeur de couleur chargée
                Console.WriteLine("Loaded Shadow Color (RGB): " + loadedShadowEffect.Color.Color.ToString());
                Console.WriteLine("Loaded Shadow Color (ARGB): " + loadedShadowEffect.Color.Argb);
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


