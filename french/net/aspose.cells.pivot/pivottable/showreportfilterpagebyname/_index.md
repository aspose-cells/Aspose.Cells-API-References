---
title: "PivotTable.ShowReportFilterPageByName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Afficher toutes les pages de filtre de rapport selon le nom des PivotFields ; le PivotField doit être situé dans les PageFields"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showreportfilterpagebyname/
---
## PivotTable.ShowReportFilterPageByName method

Affiche toutes les pages de filtre de rapport selon le nom du champ PivotField, le champ PivotField doit être situé dans les champs de page.

```csharp
public void ShowReportFilterPageByName(string fieldName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldName | String | Le nom du PivotField |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            var cells = sheet.Cells;
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
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter des champs de ligne et de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Ajouter un champ de page
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Fruit");
            pivotTable.PageFields[0].Name = "FruitFilter";
            
            // Actualiser le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Afficher les pages de filtre de rapport par nom
            pivotTable.ShowReportFilterPageByName("FruitFilter");
            
            // Enregistrez le classeur
            workbook.Save("PivotTableShowReportFilterPageByNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


