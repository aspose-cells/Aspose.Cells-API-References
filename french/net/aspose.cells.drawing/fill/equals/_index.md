---
title: "Fill.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Fill. /"
type: docs
url: /fr/net/aspose.cells.drawing/fill/equals/
---
## Fill.Equals method

/

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FillMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter une forme rectangle à la feuille de calcul
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 0, 100, 150);

                // Obtenir l’objet FillFormat depuis la forme
                FillFormat fillFormat1 = rectangle.Fill;

                // Créer une autre forme pour obtenir un deuxième objet FillFormat
                Shape oval = worksheet.Shapes.AddOval(3, 0, 0, 0, 100, 150);
                FillFormat fillFormat2 = oval.Fill;

                // Appeler la méthode Equals pour comparer les deux objets FillFormat
                bool areEqual = fillFormat1.Equals(fillFormat2);

                // Afficher le résultat de la comparaison
                Console.WriteLine($"FillFormat objects are equal: {areEqual}");

                // Démontrer également la comparaison avec null
                bool isNullEqual = fillFormat1.Equals(null);
                Console.WriteLine($"FillFormat object equals null: {isNullEqual}");

                // Enregistrez le classeur
                workbook.Save("FillEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in FillFormat Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Fill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


