---
title: "PivotArea.Filters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotArea. Obtient tous les filtres pour cette zone pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotarea/filters/
---
## PivotArea.Filters property

Obtient tous les filtres pour ce PivotArea.

```csharp
public PivotAreaFilterCollection Filters { get; }
```

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyFiltersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "SalesData";
            
            // Créer des données d'exemple
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Revenue");
            dataSheet.Cells["A2"].PutValue("Electronics");
            dataSheet.Cells["B2"].PutValue(1500);
            dataSheet.Cells["A3"].PutValue("Furniture");
            dataSheet.Cells["B3"].PutValue(800);
            dataSheet.Cells["A4"].PutValue("Electronics");
            dataSheet.Cells["B4"].PutValue(2200);

            // Créer un tableau croisé dynamique
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("A3", "SalesData!A1:B4", "RevenueAnalysis");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Configurer le champ de ligne avec des sous-totaux
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;

            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Revenue");

            // Créer une zone pivot et sélectionner des champs
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Sum of Revenue");
            pivotArea.SelectField(PivotFieldType.Row, "Category");

            // Démontrer l'utilisation de la propriété Filters
            Console.WriteLine($"Filter count: {pivotArea.Filters.Count}");
            if (pivotArea.Filters.Count > 1)
            {
                bool hasAutomaticSubtotal = pivotArea.Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
                Console.WriteLine($"Row field has automatic subtotal: {hasAutomaticSubtotal}");
            }

            workbook.Save("PivotFiltersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotAreaFilterCollection](../../pivotareafiltercollection/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


