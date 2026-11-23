---
title: "SubtotalSetting.TotalList"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SubtotalSetting. Un tableau de décalages de champs zéro‑basés indiquant les champs auxquels les sous‑totaux sont ajoutés"
type: docs
url: /fr/net/aspose.cells/subtotalsetting/totallist/
---
## SubtotalSetting.TotalList property

Un tableau de décalages de champ à base zéro, indiquant les champs auxquels les sous‑totaux sont ajoutés.

```csharp
public int[] TotalList { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertyTotalListDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configuration des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Créez et appliquez le sous‑total
            CellArea area = CellArea.CreateCellArea("A1", "B5");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 }, true, true, true);

            // Récupérez le paramètre de sous‑total pour démontrer l'utilisation de TotalList
            SubtotalSetting subtotal = worksheet.Cells.RetrieveSubtotalSetting(area);
            Console.WriteLine("TotalList contains column index: " + subtotal.TotalList[0]);
            
            // Enregistrez le classeur
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


