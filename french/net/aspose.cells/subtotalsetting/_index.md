---
title: "Classe SubtotalSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.SubtotalSetting. Représente le paramètre du sous‑total"
type: docs
url: /fr/net/aspose.cells/subtotalsetting/
---
## SubtotalSetting class

Représente le paramètre du sous-total .

```csharp
public class SubtotalSetting
```

## Propriétés

| Nom | Description |
| --- | --- |
| [GroupBy](../../aspose.cells/subtotalsetting/groupby/) { get; } | Le champ à regrouper, sous forme d'un décalage entier basé à zéro |
| [SubtotalFunction](../../aspose.cells/subtotalsetting/subtotalfunction/) { get; } | La fonction de sous‑total. |
| [SummaryBelowData](../../aspose.cells/subtotalsetting/summarybelowdata/) { get; } | Indique si un résumé doit être ajouté sous les données. |
| [TotalList](../../aspose.cells/subtotalsetting/totallist/) { get; } | Un tableau de décalages de champ à base zéro, indiquant les champs auxquels les sous‑totaux sont ajoutés. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSubtotalSettingDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter des données d'exemple à la feuille de calcul
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("Group A");
                worksheet.Cells["A3"].PutValue("Group B");
                worksheet.Cells["A4"].PutValue("Group A");
                worksheet.Cells["A5"].PutValue("Group B");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);
                worksheet.Cells["B4"].PutValue(300);
                worksheet.Cells["B5"].PutValue(400);

                // Définir la zone de cellules pour les sous‑totaux
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // Appliquer les sous‑totaux aux données
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // Récupérer le SubtotalSetting depuis la feuille de calcul
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Afficher les propriétés du SubtotalSetting
                Console.WriteLine("Subtotal Setting Properties:");
                Console.WriteLine($"GroupBy field index: {subtotalSetting.GroupBy}");
                Console.WriteLine($"Subtotal Function: {subtotalSetting.SubtotalFunction}");
                Console.WriteLine($"TotalList contains column index: {subtotalSetting.TotalList[0]}");
                Console.WriteLine($"Summary Below Data: {subtotalSetting.SummaryBelowData}");

                // Enregistrez le classeur
                workbook.Save("SubtotalSettingDemo.xlsx");
                Console.WriteLine("SubtotalSetting demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SubtotalSetting: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


