---
title: "Énum ConsolidationFunction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ConsolidationFunction enum. Représente la fonction de consolidation"
type: docs
url: /fr/net/aspose.cells/consolidationfunction/
---
## ConsolidationFunction enumeration

Représente la fonction de consolidation.

```csharp
public enum ConsolidationFunction
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Sum | `0` | Représente la fonction Sum. |
| Count | `1` | Représente la fonction Count. |
| Average | `2` | Représente la fonction Average. |
| Max | `3` | Représente la fonction Max. |
| Min | `4` | Représente la fonction Min. |
| Product | `5` | Représente la fonction Product. |
| CountNums | `6` | Représente la fonction Count Nums. |
| StdDev | `7` | Représente la fonction StdDev. |
| StdDevp | `8` | Représente la fonction StdDevp. |
| Var | `9` | Représente la fonction Var. |
| Varp | `10` | Représente la fonction Varp. |
| DistinctCount | `11` | Représente la fonction Distinct Count. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConsolidationFunctionDemo
    {
        public static void ConsolidationFunctionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Définir la zone de cellules pour le sous‑total
            CellArea cellArea = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Appliquer le sous‑total avec la fonction Sum
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Appliquer le sous‑total avec la fonction Average
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Average, new int[] { 1 });

            // Appliquer le sous‑total avec la fonction Max
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Max, new int[] { 1 });

            // Appliquer le sous‑total avec la fonction Min
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Min, new int[] { 1 });

            // Enregistrez le classeur
            workbook.Save("ConsolidationFunctionExample.xlsx");
            workbook.Save("ConsolidationFunctionExample.pdf");

            // Afficher les résultats
            Console.WriteLine("Workbook saved with subtotals applied.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


