---
title: "PivotArea.OnlyData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotArea. Indique si seules les valeurs de données dans la zone de données de la vue pour une sélection d'élément sont sélectionnées et n'incluent pas les étiquettes d'élément"
type: docs
url: /fr/net/aspose.cells.pivot/pivotarea/onlydata/
---
## PivotArea.OnlyData property

Indique si seules les valeurs de données (dans la zone de données de la vue) d’une sélection d’éléments sont sélectionnées et n’inclut pas les étiquettes d’éléments.

```csharp
public bool OnlyData { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyOnlyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Food");
            
            worksheet.Cells["B1"].PutValue("Revenue");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);
            worksheet.Cells["B4"].PutValue(2000);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configurer la zone pivot
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true; // Key property demonstration
            pivotArea.IsRowGrandIncluded = false;

            // Configuration de sortie
            Console.WriteLine("OnlyData property is set to: " + pivotArea.OnlyData);
            
            workbook.Save("PivotAreaOnlyDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


