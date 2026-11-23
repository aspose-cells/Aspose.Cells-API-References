---
title: "Range.Union"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Retourne l'union de deux plages"
type: docs
url: /fr/net/aspose.cells/range/union/
---
## Range.Union method

Retourne l'union de deux plages.

```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList Union(Range range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | Plage | La plage |

### Valeur de retour

L'union de deux plages.

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Range.UnionRanges(). Cette méthode sera supprimée 12 mois plus tard, depuis novembre 2023. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez deux plages pour démontrer Union
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:C3");

            // Remplissez des données dans les plages
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");

            try
            {
                // Appelez la méthode Union (note : il s'agit de la version obsolète)
                ArrayList unionResult = range1.Union(range2);

                Console.WriteLine("Union method executed successfully");
                Console.WriteLine($"Number of ranges in union: {unionResult.Count}");

                // Affichez les adresses de toutes les plages dans l'union
                foreach (Aspose.Cells.Range r in unionResult)
                {
                    Console.WriteLine($"Union range address: {r.Address}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("RangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


