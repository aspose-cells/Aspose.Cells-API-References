---
title: "Cells.RetrieveSubtotalSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Récupère les paramètres de sous-total de la plage"
type: docs
url: /fr/net/aspose.cells/cells/retrievesubtotalsetting/
---
## Cells.RetrieveSubtotalSetting method

Récupère les paramètres de sous-totaux de la plage.

```csharp
public SubtotalSetting RetrieveSubtotalSetting(CellArea ca)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ca | CellArea | La plage |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRetrieveSubtotalSettingWithCellAreaDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple pour les sous-totaux
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group1" : "Group2");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Créez des sous-totaux
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Récupérez les paramètres de sous-total
            SubtotalSetting setting = worksheet.Cells.RetrieveSubtotalSetting(area);

            // Paramètres de sortie
            Console.WriteLine("GroupBy: " + setting.GroupBy);
            Console.WriteLine("Function: " + setting.SubtotalFunction);
            Console.WriteLine("SummaryBelowData: " + setting.SummaryBelowData);
            Console.WriteLine("TotalList: " + string.Join(",", setting.TotalList));
        }
    }
}
```

### Voir aussi

* class [SubtotalSetting](../../subtotalsetting/)
* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


