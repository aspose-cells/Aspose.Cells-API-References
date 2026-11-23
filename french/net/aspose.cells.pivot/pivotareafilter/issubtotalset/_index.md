---
title: "PivotAreaFilter.IsSubtotalSet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotAreaFilter. Obtient quel sous-total est défini pour ce filtre"
type: docs
url: /fr/net/aspose.cells.pivot/pivotareafilter/issubtotalset/
---
## PivotAreaFilter.IsSubtotalSet method

Obtient quel sous-total est défini pour ce filtre.

```csharp
public bool IsSubtotalSet(PivotFieldSubtotalType subtotalType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Le type de fonction de sous-total. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterMethodIsSubtotalSetWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter un champ de ligne et configurer les sous-totaux
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;
            rowField.SetSubtotals(PivotFieldSubtotalType.Automatic, true);

            // Créer une zone de tableau croisé dynamique et vérifier le paramètre de sous-total
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            
            // Démontrer l'utilisation de IsSubtotalSet
            bool isSubtotalSet = pivotArea.Filters[0].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            Console.WriteLine($"Is Automatic subtotal set: {isSubtotalSet}");

            // Enregistrez le classeur
            workbook.Save("PivotSubtotalDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


