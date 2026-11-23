---
title: "Classe PivotShowValuesSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotShowValuesSetting. Représente les paramètres d'affichage des valeurs lorsque le calcul ShowDataAs est utilisé"
type: docs
url: /fr/net/aspose.cells.pivot/pivotshowvaluessetting/
---
## PivotShowValuesSetting class

Représente les paramètres d'affichage des valeurs lorsque le calcul ShowDataAs est utilisé.

```csharp
public class PivotShowValuesSetting
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/) { get; set; } | Représente le champ de base pour un calcul ShowDataAs lorsque le calcul ShowDataAs est utilisé. |
| [BaseFieldName](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldname/) { get; } | Obtient la légende du champ de base du tableau croisé dynamique. |
| [BaseItemCaption](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemcaption/) { get; } | Obtient la légende de l'élément du tableau croisé dynamique dans le champ de base. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/) { get; set; } | Représente l'index personnalisé de l'élément du tableau croisé dynamique dans le champ de base lorsque le calcul ShowDataAs est utilisé. |
| [BaseItemPositionType](../../aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/) { get; set; } | (**Obsolete.**) Représente le type de l'élément de base du tableau croisé dynamique dans le champ de base lorsque le calcul ShowDataAs est utilisé. Parce que PivotItemPosition.Custom est en lecture seule, si vous devez définir PivotItemPosition.Custom, veuillez définir l'attribut PivotField.BaseItemIndex. |
| [CalculationType](../../aspose.cells.pivot/pivotshowvaluessetting/calculationtype/) { get; set; } | (**Obsolete.**) Représente la façon d'afficher les valeurs d'un champ de données dans le rapport de tableau croisé dynamique. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotshowvaluessetting/showvaluesas/) { get; set; } | Obtient et définit la façon d'afficher les valeurs d'un champ de données dans le rapport de tableau croisé dynamique. |

## Champs

| Nom | Description |
| --- | --- |
| const [NextPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/nextpivotitem/) | Index d'élément de base spécial : utilisez l'élément suivant du tableau croisé dynamique. Valide pour les calculs "Show Values As", effectif dans Excel 2010 et versions ultérieures. |
| const [PreviousPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/previouspivotitem/) | Index d'élément de base spécial : utilisez l'élément précédent du tableau croisé dynamique. Valide pour les calculs "Show Values As", effectif dans Excel 2010 et versions ultérieures. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingDemo
    {
        public static void PivotShowValuesSettingExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            // Ajoutez un tableau croisé dynamique à la feuille de calcul
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Accéder au champ de données
            PivotField dataField = pivotTable.DataFields[0];

            // Accéder à la propriété ShowValuesSetting
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            // Définir les propriétés de PivotShowValuesSetting
            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0; // Base field index
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1; // Base item index

            // Actualiser et calculer les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotShowValuesSettingExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


