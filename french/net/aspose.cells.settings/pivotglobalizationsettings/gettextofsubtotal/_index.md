---
title: "PivotGlobalizationSettings.GetTextOfSubTotal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte du type PivotFieldSubtotalType dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/
---
## PivotGlobalizationSettings.GetTextOfSubTotal method

Obtient le texte du type [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) dans le tableau croisé dynamique.

```csharp
public virtual string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | Le [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Valeur de retour

Le texte du type donné

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfSubTotalWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 1);

            // Créer des paramètres de mondialisation
            Aspose.Cells.Settings.PivotGlobalizationSettings globalizationSettings = new Aspose.Cells.Settings.PivotGlobalizationSettings();

            // Démontrer GetTextOfSubTotal avec différents types de sous‑total
            Console.WriteLine("Sum Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Sum));
            Console.WriteLine("Count Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Count));
            Console.WriteLine("Average Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Average));
            Console.WriteLine("Max Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Max));
            Console.WriteLine("Min Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Min));

            // Enregistrer le classeur
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


