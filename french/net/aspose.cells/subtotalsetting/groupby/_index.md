---
title: "SubtotalSetting.GroupBy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SubtotalSetting. Le champ à regrouper sous forme d'un décalage entier zéro‑basé"
type: docs
url: /fr/net/aspose.cells/subtotalsetting/groupby/
---
## SubtotalSetting.GroupBy property

Le champ à regrouper, sous forme d'un décalage entier basé à zéro

```csharp
public int GroupBy { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SubtotalSettingPropertyGroupByDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
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

            try
            {
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

                // Récupérez le paramètre de sous‑total pour accéder à la propriété GroupBy
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // Affichez la valeur de la propriété GroupBy
                Console.WriteLine("GroupBy field index: " + subtotalSetting.GroupBy);

                // Enregistrez le classeur
                workbook.Save("GroupByDemo.xlsx");
                Console.WriteLine("Subtotal with GroupBy demonstrated successfully.");
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

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


