---
title: "PivotTable.PageFieldWrapCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport PivotTable"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/pagefieldwrapcount/
---
## PivotTable.PageFieldWrapCount property

Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport du tableau croisé dynamique.

```csharp
public int PageFieldWrapCount { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldWrapCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Entrer les données
            Worksheet data = workbook.Worksheets.Add("data");
            data.Cells["A1"].PutValue("Country");
            data.Cells["B1"].PutValue("Product");
            data.Cells["C1"].PutValue("Vendor");
            data.Cells["D1"].PutValue("Value");
            data.Cells["A2"].PutValue("USA");
            data.Cells["B2"].PutValue("Car");
            data.Cells["C2"].PutValue("Ford");
            data.Cells["D2"].PutValue(1200.987654321);
            data.Cells["A3"].PutValue("Japan");
            data.Cells["B3"].PutValue("Bike");
            data.Cells["C3"].PutValue("Yamaha");
            data.Cells["D3"].PutValue(985.123456789);

            // Créer un tableau croisé dynamique
            Worksheet pivot = workbook.Worksheets.Add("pivot");
            PivotTableCollection pivotTables = pivot.PivotTables;
            int index = pivotTables.Add("=data!A1:D3", "A1", "pivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Définir la propriété PageFieldWrapCount
            pivotTable.PageFieldWrapCount = 2; // Number of page fields per row
            
            // Calculer et actualiser le tableau croisé dynamique
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotTablePageFieldWrapCountDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


