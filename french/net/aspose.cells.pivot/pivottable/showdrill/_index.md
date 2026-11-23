---
title: "PivotTable.ShowDrill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient et définit si les boutons d'agrandissement/réduction sont affichés"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showdrill/
---
## PivotTable.ShowDrill property

Obtient et définit l'affichage des boutons d'expansion/réduction.

```csharp
public bool ShowDrill { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDrillDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et la remplir avec des données d'exemple
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "Pivot";
            sheet.Cells["A1"].Value = "Category";
            sheet.Cells["B1"].Value = "Value";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B4"].Value = 150;

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Activer le forage descendant et afficher les indicateurs de forage
            pivotTable.EnableDrilldown = true;
            pivotTable.ShowDrill = true;
            
            // Actualiser et calculer les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotTableShowDrillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


