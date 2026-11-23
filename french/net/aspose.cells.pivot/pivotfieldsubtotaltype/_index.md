---
title: "Enum PivotFieldSubtotalType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Pivot.PivotFieldSubtotalType enum. Description résumée pour PivotFieldSubtotalType"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldsubtotaltype/
---
## PivotFieldSubtotalType enumeration

Description résumée pour PivotFieldSubtotalType.

```csharp
[Flags]
public enum PivotFieldSubtotalType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Représente le type de sous-total Aucun. |
| Automatic | `1` | Représente le type de sous-total Automatique. |
| Sum | `2` | Représente le type de sous-total Somme. |
| Count | `4` | Représente le type de sous-total Compte. |
| Average | `8` | Représente le type de sous-total Moyenne. |
| Max | `10` | Représente le type de sous-total Max. |
| Min | `20` | Représente le type de sous-total Min. |
| Product | `40` | Représente le type de sous-total Produit. |
| CountNums | `80` | Représente le type de sous-total Count Nums. |
| Stdev | `100` | Représente le type de sous-total Écart-type. |
| Stdevp | `200` | Représente le type de sous-total Écart-type d’une population. |
| Var | `400` | Représente le type de sous-total Variance. |
| Varp | `800` | Représente le type de sous-total Variance d’une population. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSubtotalTypeDemo
    {
        public static void PivotFieldSubtotalTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Ajouter un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Définir le type de sous-total pour le champ de ligne
            PivotField rowField = pivotTable.RowFields[0];
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            rowField.SetSubtotals(PivotFieldSubtotalType.Count, true);

            // Actualiser et calculer les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotFieldSubtotalTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


