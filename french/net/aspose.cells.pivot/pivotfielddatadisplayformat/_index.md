---
title: "Enumération PivotFieldDataDisplayFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Pivot.PivotFieldDataDisplayFormat enum. Représente le format d'affichage des données dans le champ de données du tableau croisé dynamique."
type: docs
url: /fr/net/aspose.cells.pivot/pivotfielddatadisplayformat/
---
## PivotFieldDataDisplayFormat enumeration

Représente le format d'affichage des données dans le champ de données du tableau croisé dynamique.

```csharp
public enum PivotFieldDataDisplayFormat
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Normal | `0` | Représente le format d'affichage normal. |
| DifferenceFrom | `1` | Représente la différence du format d'affichage. |
| PercentageOf | `2` | Représente le pourcentage du format d'affichage. |
| PercentageDifferenceFrom | `3` | Représente la différence en pourcentage du format d'affichage. |
| RunningTotalIn | `4` | Représente le total cumulé dans le format d'affichage. |
| PercentageOfRow | `5` | Représente le pourcentage du format d'affichage de ligne. |
| PercentageOfColumn | `6` | Représente le pourcentage du format d'affichage de colonne. |
| PercentageOfTotal | `7` | Représente le pourcentage du format d'affichage total. |
| Index | `8` | Représente le format d'affichage d'index. |
| PercentageOfParentRowTotal | `9` | Représente le pourcentage du format d'affichage du total de la ligne parente. |
| PercentageOfParentColumnTotal | `10` | Représente le pourcentage du format d'affichage du total de la colonne parente. |
| PercentageOfParentTotal | `11` | Représente le pourcentage du format d'affichage du total parent. |
| PercentageOfRunningTotalIn | `12` | Représente le pourcentage du total cumulé dans le format d'affichage. |
| RankSmallestToLargest | `13` | Représente le format d'affichage du plus petit au plus grand. |
| RankLargestToSmallest | `14` | Représente le format d'affichage du plus grand au plus petit. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDataDisplayFormatDemo
    {
        public static void PivotFieldDataDisplayFormatExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ajoutez des données d'exemple
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Ajouter un tableau croisé dynamique
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Définir le style du tableau croisé dynamique
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Modifier les attributs du PivotField
            PivotField dataField = pivot.DataFields[0];
            dataField.DisplayName = "custom display name";

            // Définir DataDisplayFormat
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;

            // Actualiser et calculer les données
            pivot.RefreshData();
            pivot.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotFieldDataDisplayFormatExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


