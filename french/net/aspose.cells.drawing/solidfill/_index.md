---
title: "Classe SolidFill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.SolidFill. Encapsule l'objet qui représente le format de remplissage uni"
type: docs
url: /fr/net/aspose.cells.drawing/solidfill/
---
## SolidFill class

Encapsule l'objet qui représente le format de remplissage plein.

```csharp
public class SolidFill : Fill
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/solidfill/cellscolor/) { get; set; } | Obtient et définit l'objet [`CellsColor`](./cellscolor/). |
| [Color](../../aspose.cells.drawing/solidfill/color/) { get; set; } | Obtient ou définit la couleur. |
| [Transparency](../../aspose.cells.drawing/solidfill/transparency/) { get; set; } | Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent). |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/solidfill/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/solidfill/gethashcode/)() | Obtient le code de hachage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassSolidFillDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // Ajouter une forme rectangulaire simple à la feuille
                Shape rect = sheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);

                // Configurer la forme pour utiliser un remplissage uni
                rect.Fill.FillType = FillType.Solid;

                // Obtenir l'objet SolidFill
                SolidFill solidFill = rect.Fill.SolidFill;

                // Définir les propriétés du remplissage uni
                solidFill.Color = Color.CornflowerBlue;   // System.Drawing.Color
                solidFill.Transparency = 0.25;            // 0 = opaque, 1 = fully transparent

                // Accédez à la propriété CellsColor (lecture/écriture)
                CellsColor cellsColor = solidFill.CellsColor;
                if (cellsColor != null)
                {
                    Console.WriteLine("CellsColor object is available.");
                }
                else
                {
                    Console.WriteLine("CellsColor is null (default).");
                }

                Console.WriteLine($"SolidFill created with Color={solidFill.Color.Name}, Transparency={solidFill.Transparency}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SolidFill: {ex.Message}");
            }

            // Enregistrez le classeur pour vérifier l'apparence de la forme
            workbook.Save("DrawingClassSolidFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


