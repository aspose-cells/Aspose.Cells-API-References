---
title: "Classe PivotTableRefreshOption"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotTableRefreshOption. Représente les options de rafraîchissement de la source de données du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottablerefreshoption/
---
## PivotTableRefreshOption class

Représente les options d'actualisation de la source de données du tableau croisé dynamique.

```csharp
public class PivotTableRefreshOption
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PivotTableRefreshOption](pivottablerefreshoption/)() | Représente les options d'actualisation de la source de données du tableau croisé dynamique. |

## Propriétés

| Nom | Description |
| --- | --- |
| [IsKeepOriginalOrder](../../aspose.cells.pivot/pivottablerefreshoption/iskeeporiginalorder/) { get; set; } | Indique s'il faut conserver l'ordre original des éléments du tableau croisé dynamique comme dans l'ancienne source de données. |
| [KeepCachedLocalGroupData](../../aspose.cells.pivot/pivottablerefreshoption/keepcachedlocalgroupdata/) { get; set; } | Indique s'il faut conserver les données de groupe locales en cache si les valeurs maximale et minimale restent inchangées. La valeur par défaut est false, ce qui signifie rafraîchir le groupe avec les paramètres locaux. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablerefreshoption/reservemissingpivotitemtype/) { get; set; } | Représente la façon de réserver les éléments manquants du tableau croisé dynamique. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableRefreshOptionDemo
    {
        public static void PivotTableRefreshOptionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Ajoutez un tableau croisé dynamique à la feuille de calcul
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Créez une instance de PivotTableRefreshOption
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Rafraîchissez le tableau croisé dynamique avec les options spécifiées
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotTableRefreshOptionExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


