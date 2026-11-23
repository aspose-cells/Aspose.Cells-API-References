---
title: "PivotField.PivotItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Obtient les éléments pivot du champ PivotField"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/pivotitems/
---
## PivotField.PivotItems property

Obtient les éléments pivot du champ pivot

```csharp
public PivotItemCollection PivotItems { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPivotItemsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["A4"].Value = "A";
            worksheet.Cells["B4"].Value = 30;
            
            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Rafraîchir les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Obtenez le champ pivot et démontrez PivotItems
            PivotField field = pivotTable.RowFields[0];
            Console.WriteLine("Field Name: " + field.Name);
            Console.WriteLine("Total PivotItems: " + field.PivotItems.Count);
            
            // Afficher tous les noms des éléments pivot
            foreach (PivotItem item in field.PivotItems)
            {
                Console.WriteLine("Item Name: " + item.Name);
            }
        }
    }
}
```

### Voir aussi

* class [PivotItemCollection](../../pivotitemcollection/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


