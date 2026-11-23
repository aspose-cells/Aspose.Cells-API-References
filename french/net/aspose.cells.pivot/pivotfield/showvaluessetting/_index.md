---
title: "PivotField.ShowValuesSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Obtient les paramètres d'affichage des valeurs lorsque le calcul ShowDataAs est utilisé"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/showvaluessetting/
---
## PivotField.ShowValuesSetting property

Obtient les paramètres d'affichage des valeurs lorsque le calcul ShowDataAs est utilisé.

```csharp
public PivotShowValuesSetting ShowValuesSetting { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowValuesSettingDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 1500;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 2500;
            cells["A7"].Value = "Banana";
            cells["B7"].Value = 3500;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B7", "C10", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Ajouter des champs de ligne et de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // Configurez ShowValuesSetting pour afficher en pourcentage du total
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            
            // Calculer et actualiser le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldShowValuesSettingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotShowValuesSetting](../../pivotshowvaluessetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


