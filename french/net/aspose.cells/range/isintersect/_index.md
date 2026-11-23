---
title: "Range.IsIntersect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Indique si la plage intersecte"
type: docs
url: /fr/net/aspose.cells/range/isintersect/
---
## Range.IsIntersect method

Indique si la plage intersecte.

```csharp
public bool IsIntersect(Range range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | Plage | La plage. |

### Valeur de retour

Indique si la plage intersecte.

### Remarques

Si les deux plages ne sont pas dans la même feuille de calcul, renvoie false.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodIsIntersectWithRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer deux plages pour tester l'intersection
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B3:D8");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("C10:D15");

            try
            {
                // Vérifier si range1 intersecte range2 (devrait intersecter)
                bool result1 = range1.IsIntersect(range2);
                Console.WriteLine($"Range A1:B5 intersects with B3:D8: {result1}");

                // Vérifier si range1 intersecte range3 (ne devrait pas intersecter)
                bool result2 = range1.IsIntersect(range3);
                Console.WriteLine($"Range A1:B5 intersects with C10:D15: {result2}");

                // Remplir les plages avec différentes couleurs pour les visualiser
                Style style1 = workbook.CreateStyle();
                style1.ForegroundColor = System.Drawing.Color.LightBlue;
                style1.Pattern = BackgroundType.Solid;
                range1.SetStyle(style1);

                Style style2 = workbook.CreateStyle();
                style2.ForegroundColor = System.Drawing.Color.LightGreen;
                style2.Pattern = BackgroundType.Solid;
                range2.SetStyle(style2);

                Style style3 = workbook.CreateStyle();
                style3.ForegroundColor = System.Drawing.Color.LightPink;
                style3.Pattern = BackgroundType.Solid;
                range3.SetStyle(style3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsIntersect method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("RangeMethodIsIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


