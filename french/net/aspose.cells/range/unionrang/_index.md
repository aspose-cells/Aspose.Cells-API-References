---
title: "Range.UnionRang"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Retourne le résultat de l'union de deux plages"
type: docs
url: /fr/net/aspose.cells/range/unionrang/
---
## Range.UnionRang method

Retourne le résultat de l'union de deux plages.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Range[] UnionRang(Range range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | Plage | La plage |

### Valeur de retour

L'union de deux plages.

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Range.UnionRanges(). Cette méthode sera supprimée 12 mois plus tard à compter de mai 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using Range = Aspose.Cells.Range; // Add this alias to resolve ambiguity

    public class RangeMethodUnionRangWithRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez deux plages pour démontrer UnionRang
            Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Range range2 = worksheet.Cells.CreateRange("C3:D4");

            // Définissez quelques valeurs dans les plages pour la visualisation
            range1[0, 0].PutValue("Range1");
            range1[1, 1].PutValue("Data");
            range2[0, 0].PutValue("Range2");
            range2[1, 1].PutValue("Data");

            try
            {
                // Appelez la méthode UnionRang pour combiner les deux plages
                Range[] unionResult = range1.UnionRang(range2);

                // Affichez les informations sur le résultat de l'union
                Console.WriteLine("UnionRang method executed successfully.");
                Console.WriteLine($"Number of ranges in union: {unionResult.Length}");
                Console.WriteLine($"First union range address: {unionResult[0].Address}");
                Console.WriteLine($"Second union range address: {unionResult[1].Address}");

                // Marquez les plages d'union avec une bordure pour la visualisation
                foreach (Range r in unionResult)
                {
                    r.SetOutlineBorders(CellBorderType.Thin, System.Drawing.Color.Black);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnionRang method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("RangeMethodUnionRangWithRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


