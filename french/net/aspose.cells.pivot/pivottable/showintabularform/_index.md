---
title: "PivotTable.ShowInTabularForm"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Met en forme la PivotTable sous forme tabulaire"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showintabularform/
---
## PivotTable.ShowInTabularForm method

Mise en page du tableau croisé dynamique sous forme tabulaire.

```csharp
public void ShowInTabularForm()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInTabularFormDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Ajouter la feuille de données
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // Ajouter la feuille de tableau de pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Ajouter un tableau croisé dynamique
            int pivotIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Ajouter des champs au tableau croisé dynamique
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Afficher le tableau de pivot sous forme tabulaire
            pivotTable.ShowInTabularForm();
            
            // Actualiser et calculer les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotTableShowInTabularFormDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


