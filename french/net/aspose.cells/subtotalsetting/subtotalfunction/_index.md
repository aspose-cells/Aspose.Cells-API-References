---
title: "SubtotalSetting.SubtotalFunction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SubtotalSetting. La fonction de sous‑total"
type: docs
url: /fr/net/aspose.cells/subtotalsetting/subtotalfunction/
---
## SubtotalSetting.SubtotalFunction property

La fonction de sous‑total.

```csharp
public ConsolidationFunction SubtotalFunction { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySubtotalFunctionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group A" : "Group B");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Créez le paramètre de sous‑total en le récupérant à partir des données existantes
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Configurez le sous‑total – ces propriétés sont en lecture seule dans l'API réelle
            // Nous utiliserons donc la méthode Subtotal directement avec les paramètres
            int groupBy = 0; // Group by first column
            ConsolidationFunction function = ConsolidationFunction.Sum;
            int[] subtotalColumns = new int[] {1}; // Subtotal on second column
            
            // Appliquez les sous‑totaux
            worksheet.Cells.Subtotal(area, groupBy, function, subtotalColumns);

            // Vérifiez la propriété SubtotalFunction du paramètre récupéré
            Console.WriteLine("Subtotal Function: " + subtotalSetting.SubtotalFunction);
            
            // Enregistrez le classeur
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


