---
title: "PivotTableRefreshOption.PivotTableRefreshOption"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur PivotTableRefreshOption. Représente les options de rafraîchissement de la source de données du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottablerefreshoption/pivottablerefreshoption/
---
## PivotTableRefreshOption constructor

Représente les options d'actualisation de la source de données du tableau croisé dynamique.

```csharp
public PivotTableRefreshOption()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableRefreshOptionMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";            cells["C2"].Value = 1000;
            cells["A3"].Value = "Orange";            cells["B3"].Value = "South";            cells["C3"].Value = 2000;
            cells["A4"].Value = "Banana";            cells["B4"].Value = "East";            cells["C4"].Value = 3000;
            cells["A5"].Value = "Apple";            cells["B5"].Value = "South";            cells["C5"].Value = 4000;
            
            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Créer et configurer les options de rafraîchissement en utilisant le constructeur
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption();
            refreshOption.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Rafraîchir le tableau croisé dynamique avec des options
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotTableRefreshDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PivotTableRefreshOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


