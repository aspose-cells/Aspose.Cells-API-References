---
title: "PivotTable.MissingItemsLimit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Spécifie une valeur booléenne qui indique si les champs d’un PivotTable peuvent avoir plusieurs filtres appliqués."
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/missingitemslimit/
---
## PivotTable.MissingItemsLimit property

Spécifie une valeur booléenne qui indique si les champs d’un PivotTable peuvent avoir plusieurs filtres appliqués.

```csharp
[Obsolete("Use PivotCache.MissingItemsLimit propery  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotMissingItemLimitType MissingItemsLimit { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotCache.MissingItemsLimit. Cette méthode sera supprimée 12 mois plus tard, à partir de septembre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyMissingItemsLimitDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Données d'exemple
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 30;

            // Créez un tableau croisé dynamique et obtenez l'instance
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "E3");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value
            
            // Démontrez la propriété MissingItemsLimit
            pivotTable.MissingItemsLimit = PivotMissingItemLimitType.Max;
            
            // Rafraîchir les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            workbook.Save("PivotTableMissingItemsLimitDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotMissingItemLimitType](../../pivotmissingitemlimittype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


