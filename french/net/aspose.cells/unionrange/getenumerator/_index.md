---
title: "UnionRange.GetEnumerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode UnionRange. Obtient l'énumérateur pour les cellules de cette plage"
type: docs
url: /fr/net/aspose.cells/unionrange/getenumerator/
---
## UnionRange.GetEnumerator method

Obtient l'énumérateur des cellules de cette `Range`.

```csharp
public IEnumerator GetEnumerator()
```

### Valeur de retour

L'énumérateur de cellules

### Remarques

Lors du parcours des éléments à l'aide de l'énumérateur retourné, la collection de cellules ne doit pas être modifiée (par exemple des opérations qui entraîneraient la création d'une nouvelle Cell/Row ou la suppression d'une Cell/Row existante). Sinon, l'énumérateur pourrait ne pas être capable de parcourir toutes les cellules correctement (certains éléments pourraient être parcourus plusieurs fois ou être ignorés).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class UnionRangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez la première plage (A1:B2) et remplissez‑la avec des données
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1", "B2");
            range1[0, 0].PutValue("R1C1");
            range1[0, 1].PutValue("R1C2");
            range1[1, 0].PutValue("R2C1");
            range1[1, 1].PutValue("R2C2");

            // Créez la deuxième plage (C1:D2) et remplissez‑la avec des données
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1", "D2");
            range2[0, 0].PutValue("R1C3");
            range2[0, 1].PutValue("R1C4");
            range2[1, 0].PutValue("R2C3");
            range2[1, 1].PutValue("R2C4");

            try
            {
                // Construisez un UnionRange à partir de la première plage
                UnionRange unionRange = worksheet.Cells
                    .CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { range1 });

                // Ajoutez la deuxième plage à l'union
                unionRange = unionRange.Union("C1:D2");

                // Obtenez l'énumérateur et parcourez toutes les cellules de l'union
                IEnumerator enumerator = unionRange.GetEnumerator();
                Console.WriteLine("Enumerating cells in the UnionRange:");
                while (enumerator.MoveNext())
                {
                    Cell cell = enumerator.Current as Cell;
                    if (cell != null)
                    {
                        Console.WriteLine($"{cell.Name}: {cell.Value}");
                    }
                }

                // Enregistrez le classeur (optionnel, juste pour montrer que les données persistent)
                workbook.Save("UnionRangeGetEnumeratorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetEnumerator: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


