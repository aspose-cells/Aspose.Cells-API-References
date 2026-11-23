---
title: "Classe PivotAreaFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotAreaFilter. Représente le filtre de PivotArea pour le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotareafilter/
---
## PivotAreaFilter class

Représente le filtre de [`PivotArea`](../pivotarea/) pour [`PivotTable`](../pivottable/).

```csharp
public class PivotAreaFilter
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PivotAreaFilter](pivotareafilter/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FieldIndex](../../aspose.cells.pivot/pivotareafilter/fieldindex/) { get; } | Obtient l'index du champ dans les champs source auquel ce filtre fait référence. Une valeur de -2 indique le champ des valeurs. |
| [Selected](../../aspose.cells.pivot/pivotareafilter/selected/) { get; set; } | Indique si ce champ a une sélection. Ne fonctionne que lorsque le tableau croisé dynamique est en vue Plan. |

## Méthodes

| Nom | Description |
| --- | --- |
| [IsSubtotalSet](../../aspose.cells.pivot/pivotareafilter/issubtotalset/)(PivotFieldSubtotalType) | Obtient quel sous-total est défini pour ce filtre. |
| [SetSubtotals](../../aspose.cells.pivot/pivotareafilter/setsubtotals/)(PivotFieldSubtotalType, bool) | Sous-total pour le filtre. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configuration des données d'exemple
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            
            // Créer un tableau croisé dynamique - corriger la gestion de la valeur de retour
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Créer et configurer PivotAreaFilter
            PivotAreaFilter filter = new PivotAreaFilter();
            filter.Selected = true;
            filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            
            // Démontrer les méthodes
            bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
            Console.WriteLine($"Sum subtotal visibility set: {isSumSet}");
            
            workbook.Save("PivotAreaFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


