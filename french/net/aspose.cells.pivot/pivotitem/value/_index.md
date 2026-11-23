---
title: "PivotItem.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotItem. Obtient la valeur de l'élément de tableau croisé"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/value/
---
## PivotItem.Value property

Obtient la valeur de l'élément pivot

```csharp
public object Value { get; }
```

### Exemples

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyValueDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Obtenez le champ du tableau croisé
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Traiter les éléments du tableau croisé
            List<string> valuesToShow = new List<string> { "Apple", "Banana" };
            
            Console.WriteLine("Pivot Items Before Filtering:");
            PrintPivotItems(pivotField);

            // Filtrer les éléments du tableau croisé en fonction de la propriété Value
            for (int i = 0; i < pivotField.PivotItems.Count; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                string itemValue = item.Value?.ToString() ?? "";
                
                if (!valuesToShow.Contains(itemValue))
                {
                    item.IsHidden = true;
                }
            }

            Console.WriteLine("\nPivot Items After Filtering:");
            PrintPivotItems(pivotField);
        }

        private static void PrintPivotItems(PivotField pivotField)
        {
            for (int i = 0; i < pivotField.PivotItems.Count; i++)
            {
                PivotItem item = pivotField.PivotItems[i];
                Console.WriteLine($"Name: {item.Name}, Value: {item.Value}, Hidden: {item.IsHidden}");
            }
        }
    }
}
```

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


