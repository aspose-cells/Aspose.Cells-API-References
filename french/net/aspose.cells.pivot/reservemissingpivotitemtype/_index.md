---
title: "Enum ReserveMissingPivotItemType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Pivot.ReserveMissingPivotItemType enum. Représente la façon de conserver les éléments pivot manquants"
type: docs
url: /fr/net/aspose.cells.pivot/reservemissingpivotitemtype/
---
## ReserveMissingPivotItemType enumeration

Représente la façon de conserver les éléments manquants du tableau croisé dynamique.

```csharp
public enum ReserveMissingPivotItemType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | Supprime les anciens éléments pivot manquants et réserve les éléments supprimés de la nouvelle source de données comme éléments manquants. |
| All | `1` | Réserve tous les éléments manquants. |
| None | `2` | Supprime tous les éléments pivot manquants. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class ReserveMissingPivotItemTypeDemo
    {
        public static void ReserveMissingPivotItemTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un PivotTable à la feuille de calcul
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Ajoutez des champs au PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Définissez l'option ReserveMissingPivotItemType
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calculez le PivotTable avec les options spécifiées
            pivotTable.CalculateData(calculateOption);

            // Rafraîchissez le PivotTable
            pivotTable.RefreshData();

            // Enregistrez le classeur
            workbook.Save("ReserveMissingPivotItemTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


