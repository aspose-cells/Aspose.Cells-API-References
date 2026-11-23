---
title: "GradientFill.SetGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GradientFill. Définit le type de remplissage de dégradé et la direction"
type: docs
url: /fr/net/aspose.cells.drawing/gradientfill/setgradient/
---
## GradientFill.SetGradient method

Définir le type et la direction du remplissage en dégradé.

```csharp
public void SetGradient(GradientFillType type, double angle, GradientDirectionType direction)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | GradientFillType | Type de remplissage de dégradé. |
| angle | Double | L'angle. S'applique uniquement pour GradientFillType.Linear. |
| direction | GradientDirectionType | Le type de direction. S'applique uniquement pour GradientFillType.Radial et GradientFillType.Rectangle. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GradientFillMethodSetGradientWithGradientFillTypeDoubleGradientDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme pour appliquer un remplissage en dégradé
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 100);

            try
            {
                // Obtenir le dégradé de remplissage de la forme
                GradientFill gradientFill = shape.Fill.GradientFill; // Fixed property name from Gradient to GradientFill
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Appeler SetGradient avec des paramètres spécifiques : remplissage linéaire, 90 degrés, direction FromCenter
                gradientFill.SetGradient(GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter);
                
                Console.WriteLine("SetGradient method executed successfully with parameters (GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGradient method: {ex.Message}");
            }
            
            // Enregistrez le classeur pour démontrer l'effet
            workbook.Save("GradientFillSetGradientDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientFillType](../../gradientfilltype/)
* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


