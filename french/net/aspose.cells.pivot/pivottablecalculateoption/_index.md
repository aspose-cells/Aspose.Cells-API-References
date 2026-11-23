---
title: "Classe PivotTableCalculateOption"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotTableCalculateOption. Représente les options de calcul des données du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottablecalculateoption/
---
## PivotTableCalculateOption class

Représente les options de calcul des données du tableau croisé dynamique.

```csharp
public class PivotTableCalculateOption
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PivotTableCalculateOption](pivottablecalculateoption/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [RefreshCharts](../../aspose.cells.pivot/pivottablecalculateoption/refreshcharts/) { get; set; } | Indique si les graphiques de rafraîchissement sont basés sur ce tableau croisé dynamique. |
| [RefreshData](../../aspose.cells.pivot/pivottablecalculateoption/refreshdata/) { get; set; } | Indique si la source de données de rafraîchissement du tableau croisé dynamique. |
| [RefreshOption](../../aspose.cells.pivot/pivottablecalculateoption/refreshoption/) { get; set; } | Obtient et définit les options de rafraîchissement de la source de données vers le cache du tableau croisé dynamique. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/) { get; set; } | Représente la façon de réserver les éléments manquants du tableau croisé dynamique. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionDemo
    {
        public static void PivotTableCalculateOptionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // Ajoutez un tableau croisé dynamique à la feuille de calcul
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Créer un objet PivotTableCalculateOption
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calculer les données du tableau croisé dynamique avec les options spécifiées
            pivotTable.CalculateData(calculateOption);

            // Enregistrez le classeur
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


