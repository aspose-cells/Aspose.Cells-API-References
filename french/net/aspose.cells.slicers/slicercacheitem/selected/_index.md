---
title: "SlicerCacheItem.Selected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SlicerCacheItem. Indique si le SlicerCacheItem est sélectionné ou non"
type: docs
url: /fr/net/aspose.cells.slicers/slicercacheitem/selected/
---
## SlicerCacheItem.Selected property

Indique si le [`SlicerCacheItem`](../) est sélectionné ou non.

```csharp
public bool Selected { get; set; }
```

### Remarques

Veuillez utiliser la méthode [`SelectItems`](../../slicer/selectitems/) à la place si vous souhaitez sélectionner un élément. Car cette opération de rafraîchissement entraîne de mauvaises performances en raison du rechargement complet des données à chaque changement de sélection.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemPropertySelectedDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ajouter un slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Aspose.Cells.Slicers.Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Accéder aux éléments du cache de segment
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem item = slicer.SlicerCache.SlicerCacheItems[i];
                
                // Sélectionner le premier élément, désélectionner les autres
                if (i == 0)
                {
                    item.Selected = true;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
                else
                {
                    item.Selected = false;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
            }

            // Enregistrez le classeur
            workbook.Save("SlicerCacheItemSelectedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


