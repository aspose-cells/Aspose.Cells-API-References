---
title: "PivotItem.IsDetailHidden"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotItem. Obtient et définit si le détail de cet élément pivot est masqué"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/isdetailhidden/
---
## PivotItem.IsDetailHidden property

Obtient et définit si le détail de cet élément pivot est masqué.

```csharp
public bool IsDetailHidden { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsDetailHiddenDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Fruit");
            sheet.Cells["A4"].PutValue("Vegetable");
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Item");
            sheet.Cells["B2"].PutValue("Apple");
            sheet.Cells["B3"].PutValue("Orange");
            sheet.Cells["B4"].PutValue("Carrot");
            sheet.Cells["B5"].PutValue("Potato");
            sheet.Cells["C1"].PutValue("Amount");
            sheet.Cells["C2"].PutValue(10);
            sheet.Cells["C3"].PutValue(15);
            sheet.Cells["C4"].PutValue(20);
            sheet.Cells["C5"].PutValue(25);

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter des champs de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            
            // Actualiser et calculer les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Masquez les détails pour la catégorie "Fruit"
            pivotTable.RowFields[0].PivotItems["Fruit"].IsDetailHidden = true;
            
            // Enregistrez le classeur
            wb.Save("PivotItemIsDetailHiddenDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


