---
title: "PivotFilter.EvaluationOrder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFilter. Obtient l'ordre d'évaluation du filtre pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/evaluationorder/
---
## PivotFilter.EvaluationOrder property

Obtient l'ordre d'évaluation du filtre pivot.

```csharp
public int EvaluationOrder { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyEvaluationOrderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Remplissez des données d'exemple
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;
            cells["B5"].Value = 400;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivots[pivotIndex];
            
            // Ajouter des champs
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ajouter un filtre pivot
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            
            // Définir les propriétés du filtre, y compris EvaluationOrder
            filter.EvaluationOrder = 1;
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Actualiser le tableau croisé dynamique
            pivot.RefreshData();
            pivot.CalculateData();

            // Enregistrer le classeur
            book.Save("PivotFilterEvaluationOrderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


