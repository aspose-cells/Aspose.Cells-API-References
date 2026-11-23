---
title: "PivotField.Items"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Obtient toutes les étiquettes des éléments pivot dans ce champ"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/items/
---
## PivotField.Items property

Obtient toutes les étiquettes des éléments pivot dans ce champ.

```csharp
public string[] Items { get; }
```

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyItemsDemo
    {
        public static void Run()
        {
            // Créez un classeur et ajoutez des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter un champ pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Démontrer la propriété Items
            string[] items = pivotField.Items;
            Console.WriteLine("Pivot Field Items:");
            foreach (string item in items)
            {
                Console.WriteLine(item);
            }
            
            // Définir l'élément de page actuel
            ArrayList list = new ArrayList(items);
            if (list.Contains("Apple"))
            {
                pivotField.CurrentPageItem = (short)list.IndexOf("Apple");
                Console.WriteLine("Current page item set to: Apple");
            }
            
            pivotTable.CalculateData();
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


