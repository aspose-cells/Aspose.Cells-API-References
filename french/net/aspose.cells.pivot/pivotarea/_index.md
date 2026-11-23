---
title: "Class PivotArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotArea. Présente la zone sélectionnée du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotarea/
---
## PivotArea class

Présente la zone sélectionnée du tableau croisé dynamique.

```csharp
public class PivotArea
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PivotArea](pivotarea/)(PivotTable) | Présente la zone sélectionnée du PivotTable. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AxisType](../../aspose.cells.pivot/pivotarea/axistype/) { get; set; } | Obtient et définit la région du PivotTable à laquelle cette règle s'applique. |
| [Filters](../../aspose.cells.pivot/pivotarea/filters/) { get; } | Obtient tous les filtres pour ce PivotArea. |
| [IsColumnGrandIncluded](../../aspose.cells.pivot/pivotarea/iscolumngrandincluded/) { get; set; } | Indique si le total général de la colonne est inclus. |
| [IsOutline](../../aspose.cells.pivot/pivotarea/isoutline/) { get; set; } | Indique si la règle se réfère à une zone en mode plan. |
| [IsRowGrandIncluded](../../aspose.cells.pivot/pivotarea/isrowgrandincluded/) { get; set; } | Indique si le total général de la ligne est inclus. |
| [OnlyData](../../aspose.cells.pivot/pivotarea/onlydata/) { get; set; } | Indique si seules les valeurs de données (dans la zone de données de la vue) d’une sélection d’éléments sont sélectionnées et n’inclut pas les étiquettes d’éléments. |
| [OnlyLabel](../../aspose.cells.pivot/pivotarea/onlylabel/) { get; set; } | Indique si seules les étiquettes de données d’une sélection d’éléments sont sélectionnées. |
| [RuleType](../../aspose.cells.pivot/pivotarea/ruletype/) { get; set; } | Obtient et définit le type de règle de sélection. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetCellAreas](../../aspose.cells.pivot/pivotarea/getcellareas/)() | Obtient les zones de cellules de cette zone de tableau croisé dynamique. |
| [Select](../../aspose.cells.pivot/pivotarea/select/)(PivotFieldType, int, PivotTableSelectionType) | Sélectionnez la zone avec des filtres. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield)(PivotFieldType, PivotField) | Sélectionnez un champ dans la région comme zone. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield_1)(PivotFieldType, string) | Sélectionnez un champ dans la région comme zone. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaDemo
    {
        public static void PivotAreaExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Ajoutez un tableau croisé dynamique à la feuille de calcul
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Créez une instance de PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);

            // Définissez les propriétés du PivotArea
            pivotArea.OnlyData = true;
            pivotArea.OnlyLabel = false;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.IsOutline = false;

            // Utilisez la méthode Select pour sélectionner une zone spécifique
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Enregistrez le classeur
            workbook.Save("PivotAreaExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


