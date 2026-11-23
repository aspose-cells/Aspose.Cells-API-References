---
title: "PivotTable.ShowInCompactForm"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Met en forme la vue du tableau croisé dynamique en format compact"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showincompactform/
---
## PivotTable.ShowInCompactForm method

Mise en page de la vue du tableau croisé dynamique sous forme compacte.

```csharp
public void ShowInCompactForm()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInCompactFormDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir des données source
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Product");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Electronics");
            sourceSheet.Cells["B2"].PutValue("Laptop");
            sourceSheet.Cells["C2"].PutValue(1200);
            
            sourceSheet.Cells["A3"].PutValue("Electronics");
            sourceSheet.Cells["B3"].PutValue("Phone");
            sourceSheet.Cells["C3"].PutValue(800);
            
            sourceSheet.Cells["A4"].PutValue("Furniture");
            sourceSheet.Cells["B4"].PutValue("Chair");
            sourceSheet.Cells["C4"].PutValue(150);
            
            sourceSheet.Cells["A5"].PutValue("Furniture");
            sourceSheet.Cells["B5"].PutValue("Table");
            sourceSheet.Cells["C5"].PutValue(300);

            // Créer une feuille de calcul de tableau croisé dynamique
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Ajouter un tableau croisé dynamique
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("=Sheet1!A1:C5", "A3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Ajouter des champs aux zones
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Définir le tableau croisé dynamique pour affichage en format compact
            pivotTable.ShowInCompactForm();
            
            // Calculer les données et actualiser
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Enregistrez le classeur
            workbook.Save("PivotTableCompactFormDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


