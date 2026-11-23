---
title: "PivotShowValuesSetting.CalculationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotShowValuesSetting. Représente la façon d'afficher les valeurs d'un champ de données dans le rapport pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotshowvaluessetting/calculationtype/
---
## PivotShowValuesSetting.CalculationType property

Représente la façon d'afficher les valeurs d'un champ de données dans le rapport pivot.

```csharp
[Obsolete("Use PivotShowValuesSetting.ShowValuesAs property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldDataDisplayFormat CalculationType { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotShowValuesSetting.ShowValuesAs. Cette méthode sera supprimée 12 mois plus tard, à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotShowValuesSettingPropertyCalculationTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Ajouter un champ de données et définir le type de calcul
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.RankLargestToSmallest;

            // Calculez les données et enregistrez
            pivotTable.CalculateData();
            workbook.Save("PivotShowValuesSettingPropertyCalculationTypeDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


