---
title: "PivotTable.RowHeaderCaption"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient et définit la légende personnalisée de l'en-tête de ligne dans ce PivotTable"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/rowheadercaption/
---
## PivotTable.RowHeaderCaption property

Obtient et définit la légende personnalisée de l'en-tête de ligne dans ce PivotTable.

```csharp
public string RowHeaderCaption { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Ajouter la feuille de données
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Ajoutez des données d'exemple
            var cells = dataSheet.Cells;
            cells["A1"].PutValue("State");
            cells["B1"].PutValue("City");
            cells["C1"].PutValue("Population");
            
            cells["A2"].PutValue("TN");
            cells["B2"].PutValue("Chennai");
            cells["C2"].PutValue("50");
            
            cells["A3"].PutValue("KL");
            cells["B3"].PutValue("Cochin");
            cells["C3"].PutValue("70");
            
            // Ajouter une feuille de calcul de tableau croisé dynamique
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Ajouter un tableau croisé dynamique et obtenir son indice
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C3", 
                "A3", 
                "PivotTable");
            
            // Obtenir l'instance du tableau croisé dynamique
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Configurer le tableau croisé dynamique
            pivotTable.RowHeaderCaption = "State"; // Demonstrating RowHeaderCaption property
            pivotTable.AddFieldToArea(PivotFieldType.Row, "State");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Population");
            
            // Enregistrez le classeur
            workbook.Save("PivotTableWithRowHeaderCaption.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


